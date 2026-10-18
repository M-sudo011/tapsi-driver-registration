# Tapsi Driver — Login and Registration Prototype

A static, mobile-first interactive prototype for the proposed **Option A** driver onboarding flow.

## Screens
1. Vehicle selection — car or motorcycle (matching the existing entry flow).
2. Phone-number login with an additional CTA: «هنوز راننده تپسی نیستید؟ همین حالا ثبت‌نام کنید».
3. Six-digit OTP verification (**demo code: 123456**).
4. Login success.
5. Registration destination: https://join.tapsi.ir/driver.

## Preview locally
Open `index.html` in a browser. No build tools or package installation are needed.

## Publish via GitHub Pages
1. Open **Settings → Pages** in the repository.
2. Under **Build and deployment**, select **Deploy from a branch**.
3. Select **main** and **/(root)**, then click **Save**.
4. After deployment completes, visit the Pages URL shown in Settings.

## Limitations
- This is a UX prototype, not a production authentication app.
- No SMS is sent or user data persisted to a server.
- Any valid Iranian mobile number works with simulated code `123456`.
- The registration destination opens the real Tapsi page in a new browser tab. The production Android implementation can use a native WebView; an arbitrary remote website cannot reliably be embedded in an iframe because of framing policies.
- Illustrative vehicle icons and a stylized Tapsi wordmark are included inline, not official design-system assets.
