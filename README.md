**Languages:** [Türkçe](README-tr.md) · English

# BilgiKutusu Go

**The lowest-tier, basic starter package of the BilgiKutusu family.**

Access files on your Raspberry Pi from a phone or computer connected to the same local network. No internet is required to open pre-saved content; only a local network connection to the device is needed.

## What does it do?

- Browse folders and filter by name inside the open folder.
- Open and download files.
- Turkish, mobile-friendly web interface.
- Optional autostart and Wi-Fi profile setup.

Does not include AI or pre-loaded book, movie, map, or Wikipedia collections. Go is the most basic package; Plus is the mid-tier, and Pro is the top package.

## Quick start

On a Linux/Raspberry Pi device with Python 3.9 or newer, open a terminal in this folder:

```bash
bash baslat.sh
```

Open **http://127.0.0.1:8090** in the browser on the same device. Use `Ctrl+C` to stop.

To run automatically every time the Pi boots and access it from a phone on the same network:

```bash
sudo bash install/kur.sh
```

After installation, find the Pi's address with `hostname -I`, then open `http://PI_IP_ADDRESS:8090` on your phone. The installer uses separate Go folders and does not modify existing BilgiKutusu files or network settings.

## Clean folder structure

| File / folder | Contents |
| --- | --- |
| `baslat.sh` | Quick trial without installation |
| `app/` | Python code and web interface |
| `config/` | Local trial settings |
| `content/` | Sample folders; space for your own files |
| `install/` | Install, update, status, uninstall, and Wi-Fi tools |
| `docs/` | User guides and TXT explanations |
| `tests/` | Automated tests |
| `LICENSE` | Full license text |

**Guides:** [First steps](docs/BASLA.txt) · [Installation](docs/KURULUM.md) · [Detailed usage](docs/KULLANIM.md) · [Wi-Fi](docs/WIFI.md)

## Test status

```bash
python3 -m unittest discover -s testler -v
```

File access tests pass. Raspberry Pi/Wi-Fi and visual browser testing have not been performed yet. [Test details](docs/TESTLER.md).

## Privacy

The package contains no API keys or hardcoded passwords. Full name is retained for license and developer attribution. [Privacy details](docs/GIZLILIK.md).

## License and contribution

Free for personal and educational use. Prior written permission is required for commercial use. [License](LICENSE) · [Contribution terms](docs/KATKI.md).

Due to the commercial use restriction, this is not an OSI-compliant open-source license. Intended for use on a trusted local network; does not provide user accounts or HTTPS.

---

> **方針:**
> プロジェクトを立ち上げただけで責任を放棄し、「Linuxが使えるから」という理由で作業や後処理をすべて押し付ける行為には一切応じない。私は誰の便利屋でもない。各自が自分の尻拭いをすること。これ以上の関与は終了する。


