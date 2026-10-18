# Tapsi Driver — Login and Registration Prototype

A static, mobile-first interactive prototype for the proposed **Option A** driver onboarding flow.

## Screens
1. Vehicle selection — car or motorcycle. The vehicle icons and Tapsi wordmark are cropped from the reference screenshots supplied for this prototype.
2. Phone-number login with a secondary registration link: **«هنوز راننده تپسی نیستید؟ ثبت‌نام کنید»**.
3. Six-digit OTP verification (**demo code: 123456**).
4. Simulated login success.

## Registration link

The registration CTA on the phone screen directly opens:

https://join.tapsi.ir/driver

The live registration page opens in a new tab with no intermediate mockup screen. In the Android app implementation, the same URL can be opened in an app-owned WebView.

## Preview locally

Open `index.html` in a browser. No build tools or package installation are needed.

## GitHub Pages

**Settings → Pages → Build and deployment → Deploy from a branch → main / (root) → Save.**

Deployed URL: https://m-sudo011.github.io/tapsi-driver-registration/

## Notes and limitations

- UX demo only. It does not communicate with a real authentication server or send real SMS.
- Simulated login uses any valid Iranian mobile number and OTP `123456`.
- Persian typography uses locally available `IRANSansX` / `IRANSans`, falling back to Google Fonts Estedad, then Tahoma. The exact proprietary production font has not been supplied.
- Cropped vehicle/logo assets come from the user's provided screenshot. These are raster reference images and should be swapped for official design-system assets before production use.
- The registration page is an external destination rather than an embedded iframe to avoid cross-origin embedding restrictions.
