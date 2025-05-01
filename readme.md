# InsiderTweak

![Screenshot of InsiderTweak](https://i.imgur.com/YTtU1to.png)

**InsiderTweak Enroll** is a powerful offline tool for enrolling your Windows device into the Windows Insider Program—without needing a Microsoft account or submitting any participation request. Perfect for those who value privacy, control over their update process, or simply prefer to skip the official request workflow.

- [Русский](readme.ru.md)
- [简体中文](readme.zh.md)

---

## Key Features

- **Offline Enrollment**  
  Enroll into Canary, Dev, Beta or Release Preview channels via direct registry edits—no online approval required.

- **Fast Update Check**  
  Instantly query your current Insider branch and build number with one menu option.

- **Multilingual Interface**  
  Available in English, Russian and Simplified Chinese. Switch languages on the fly within the script.

- **Privacy-First**  
  No telemetry opt-in prompts, no web sign-ins—your data stays on your machine.

---

## Requirements

- Windows 11 or Windows 10 (1809 or newer).  
- Administrative privileges.

---

## Usage

1. Right-click **InsiderTweakEnroll.cmd** → **Run as Administrator**.  
2. Select a channel or choose “Check Updates” / “Change Language”.  
3. If prompted, reboot to enable Microsoft Flight Signing.  
4. Ensure your diagnostic data is set to **Full** in *Settings → Privacy &amp; feedback*.

---

## How It Works

By setting undocumented registry flags (e.g. `TestFlags=0x20`), the script disables online Insider-service checks and applies your chosen configuration locally. Because Windows Update does not verify online enrollment, you’ll receive Insider builds simply by having the correct registry values.

---

## Restoring Defaults

Run the “Stop receiving Insider builds” option to remove all Insider settings and disable Flight Signing. A reboot is required.

---

## License

MIT License. See [LICENSE](LICENSE) for details.

---
