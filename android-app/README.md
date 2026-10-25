# Android-версия «Мои квартиры»

Это обёртка (Capacitor) над тем же `index.html`. Руками её собирать не нужно:
файл `.github/workflows/android.yml` на GitHub сам собирает и подписывает APK
и выкладывает его в раздел Releases.

- Новая версия: поменяй `const VERSION='…'` в `index.html` и загрузи файл в репозиторий — сборка запустится сама.
- Ссылка на последнюю версию: `https://github.com/ВЛАДЕЛЕЦ/РЕПОЗИТОРИЙ/releases/latest/download/kvartiry.apk`
- Ключ подписи хранится только в секретах GitHub (ANDROID_KEYSTORE_BASE64, ANDROID_KEYSTORE_PASSWORD, ANDROID_KEY_ALIAS).
  Без него обновления поверх установленного приложения не встанут.
