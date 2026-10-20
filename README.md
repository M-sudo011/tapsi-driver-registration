# Tapsi Driver — Login and Registration Prototype

A static, mobile-first interactive prototype for the proposed **Option A** driver onboarding flow.

## Screens
1. Vehicle selection — car or motorcycle. The vehicle cards and Tapsi wordmark use the higher-resolution images supplied for this prototype (embedded as optimized WebP data URIs).
2. Phone-number login with a clearly visible secondary registration card: **«هنوز راننده تپسی نیستید؟ ثبت‌نام راننده جدید»**. The terms link is below both actions.
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
- The logo and vehicle graphics are higher-resolution, user-supplied assets embedded as optimized WebP. For production, reference the official design-system asset files directly.
- The registration page is an external destination rather than an embedded iframe to avoid cross-origin embedding restrictions.
