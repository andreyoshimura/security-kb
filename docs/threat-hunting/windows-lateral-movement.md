# 🪟 Windows Lateral Movement

## 🔑 Explicit Credentials

Source page:
- [Windows Lateral Movement via Explicit Credentials](https://digitalguardian.com/blog/seek-evil-and-ye-shall-find-guide-cyber-threat-hunting-operations)

## 🪟 Windows Event Logs

- Event ID 4648
- Event ID 552

## 📝 Notes

- Check audit policy to ensure events are generated.
- Collect from both servers and endpoints.
- Whitelist recurring authorized activity and keep that whitelist updated.

## 🔗 Related

- [Detecting Lateral Movement in Windows Event Logs](https://www.first.org/resources/papers/conf2016/FIRST-2016-105.pdf)
- [CAR-2013-02-008: Simultaneous Logons on a Host](https://car.mitre.org/wiki/CAR-2013-02-008)
- [CAR-2013-02-012: User Logged in to Multiple Hosts](https://car.mitre.org/wiki/CAR-2013-02-012)
- [CAR-2016-04-004: Successful Local Account Login](https://car.mitre.org/wiki/CAR-2016-04-004)
- [PsExec Events](psexec-events.md)
