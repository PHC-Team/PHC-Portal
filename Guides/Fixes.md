# SteamTools Troubleshooting Guide

## No Internet Connection (Manifest Fetching Errors)

### Recommended Fix (Semi-Permanent)

Install and apply the **CloudRedirect SteamTools Patch**:

https://github.com/Selectively11/CloudRedirect/releases

This is the recommended solution for resolving most manifest fetching and **"No Internet Connection"** errors.

---

## Steam Cloud Not Working

If Steam Cloud is not working for a SteamTools game, run the following PowerShell command:

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -Command "Invoke-WebRequest 'https://raw.githubusercontent.com/Smealm/steamtools-stuff/refs/heads/main/steamtools-nocloud.ps1' -UseBasicParsing | Invoke-Expression"
```

**Important:** This fix only applies to the games that are currently installed. If you install another SteamTools game later, you'll need to run the command again.

---

## Game Shows "Purchase" or Doesn't Appear in Your Library

SteamTools relies on its own servers to fetch manifests. If those servers are unavailable, or if Steam has recently updated, games may temporarily appear as **"Purchase"** or may not show up in your library.

Before troubleshooting, keep in mind that the issue may simply be temporary.

### Troubleshooting

#### 1. Update Steam

Make sure you're using the latest stable version of Steam and are **not** enrolled in the Steam Beta.

To check:

* Open **Help → About Steam**.
* If an update is available, click **Steam → Check for Steam Client Updates**.

---

#### 2. Update SteamTools

Make sure you're using the latest SteamTools version.

It is recommended to install or update the SteamTools DLLs using the PowerShell script provided on the official SteamTools website.

Avoid updating through the floating SteamTools icon, as it may install an older version of the DLLs.

---

#### 3. Install CloudRedirect

Using CloudRedirect can resolve several known SteamTools issues.

---

#### 4. Verify the SteamTools DLLs

Check that the required DLL files are still present in your Steam installation directory.

Current DLLs include:

* `xinput1_4.dll`
* `dwmapi.dll`

If your antivirus removed them, restore the files and add them to your antivirus exclusions.

---

#### 5. Verify the Plugin Files

Open:

```text
Steam\config\st-plugin
```

Confirm that a `<appid>.lua` file exists for the game you're trying to launch, where `<appid>` is the Steam App ID of that game.

---

#### 6. Check for Network or Regional Restrictions

Some Internet Service Providers (ISPs) may block connections to the SteamTools servers.

In some regions, SteamTools itself may also restrict access.

If you suspect this is the case, try connecting through a VPN. A **Singapore** server is generally recommended.

---

## Still Need Help?

If none of the solutions above resolve your issue, feel free to ask for assistance in our Discord server. Be sure to describe your problem and include any error messages you've encountered so we can help you more effectively.
