# 링크 보관함 — 개인정보처리방침

**앱 이름:** 링크 보관함
**패키지 이름:** `com.codebrunch.url`
**시행일:** 2026년 8월 15일
**문의:** codebrunch27@gmail.com

> 이 문서는 [https://codebrunch.github.io/urlnote/](https://codebrunch.github.io/urlnote/) 에서도 같은 내용으로 볼 수 있습니다.
> (영문본은 아래 [English](#english) 참조)

---

## 한 줄 요약

이 앱은 **개인정보를 수집하지 않습니다.** 저장한 링크는 기기 안에만 있고, 개발자에게 전송되지 않습니다. 개발자는 서버를 운영하지 않습니다.

---

## 1. 앱이 저장하는 정보

아래 정보는 **오직 사용자의 기기 안에만** 저장되며, 외부로 전송되지 않습니다.

| 항목 | 설명 |
|---|---|
| 링크 주소(URL) | 사용자가 다른 앱에서 공유하거나 직접 입력한 주소 |
| 제목·썸네일 주소·파비콘 주소 | 해당 웹페이지에서 자동으로 읽어온 값 |
| 메모 | 사용자가 직접 입력한 내용 |
| 태그 | 사용자가 만든 분류 이름과 색상 |
| 북마크·읽음 표시·저장 시각 | 목록 정리를 위한 상태값 |
| 앱 설정 | 저장 모드, 썸네일 표시, 정렬 기준, 테마, 보관 기간 |
| 썸네일 이미지 캐시 | 최대 100MB. 오래된 것부터 자동 삭제됩니다 |

이 앱은 **계정이나 로그인이 없습니다.** 이름, 이메일, 전화번호, 주소록, 위치, 기기 식별자 등 개인을 알아볼 수 있는 정보는 어떤 것도 수집하지 않습니다.

## 2. 앱이 하지 않는 일

- 개발자가 운영하는 서버로 데이터를 보내지 않습니다. **개발자는 서버를 운영하지 않습니다.**
- 분석 도구(애널리틱스)나 광고 SDK를 사용하지 않습니다.
- 사용자 활동을 추적하지 않습니다.
- 어떤 정보도 제3자에게 판매하거나 제공하지 않습니다.

## 3. 앱이 인터넷에 접속하는 경우

이 앱은 **딱 하나의 이유로만** 인터넷에 접속합니다.

**링크를 저장하면, 그 링크의 웹사이트에 직접 접속해 제목과 미리보기 이미지를 읽어옵니다.**

이때 알아두실 점이 있습니다.

- 접속 대상은 **사용자가 저장한 바로 그 웹사이트**입니다. 개발자의 서버를 거치지 않습니다.
- 따라서 그 웹사이트는, 사용자가 브라우저로 그 페이지를 직접 열었을 때와 마찬가지로 **사용자의 IP 주소와 브라우저 정보(User-Agent)를 받게 됩니다.**
- 미리보기 이미지는 그 페이지가 지정한 주소(대개 해당 사이트나 CDN)에서 내려받습니다.
- 해당 웹사이트가 사용자의 정보를 어떻게 다루는지는 **그 웹사이트의 개인정보처리방침**을 따르며, 개발자가 관여하거나 통제할 수 없습니다.

인터넷 접속이 불가능하면 링크는 주소만 저장되고, 나중에 연결되었을 때 미리보기를 다시 가져옵니다.

## 4. 백업

기기에서 **Android 자동 백업(Google Drive 백업)** 이 켜져 있으면, 저장한 링크와 앱 설정이 **사용자 본인의 Google 계정** 백업에 포함될 수 있습니다.

- 이 백업은 Google이 제공하는 기능이며, 개발자는 그 내용에 접근할 수 없습니다.
- 원하지 않으시면 기기의 *설정 → 시스템 → 백업* 에서 끌 수 있습니다.
- 이 백업에 대해서는 [Google 개인정보처리방침](https://policies.google.com/privacy)이 적용됩니다.

## 5. 앱이 요청하는 권한

| 권한 | 사용 목적 |
|---|---|
| 인터넷(INTERNET) | 링크의 제목·미리보기 이미지를 가져오기 위해 |
| 네트워크 상태 확인(ACCESS_NETWORK_STATE) | 연결이 있을 때만 미리보기를 가져오기 위해 |
| WAKE_LOCK, RECEIVE_BOOT_COMPLETED, FOREGROUND_SERVICE | 안드로이드 표준 작업 예약 라이브러리(WorkManager)가 미리보기 가져오기와 오래된 링크 정리를 백그라운드에서 실행하기 위해 자동으로 추가하는 권한입니다 |

카메라, 위치, 연락처, 저장소 접근 권한 등은 요청하지 않습니다.

## 6. 정보의 보관과 삭제

- 저장한 링크는 사용자가 지우기 전까지 기기에 남습니다.
- 앱 안에서 링크를 개별 삭제할 수 있습니다.
- 설정에서 **보관 기간**(1주일·1개월·6개월·1년)을 정하면 그보다 오래된 링크가 자동으로 삭제됩니다. 다만 **북마크한 링크는 기간이 지나도 삭제되지 않습니다.**
- 설정에서 이미지 캐시를 비울 수 있습니다.
- **앱을 삭제하면 저장된 모든 데이터가 기기에서 함께 삭제됩니다.** (위 4항의 Google 계정 백업은 별도입니다)

개발자가 보관하는 사용자 데이터가 없으므로, 개발자에게 열람·정정·삭제를 요청할 대상 자체가 존재하지 않습니다.

## 7. 아동

이 앱은 아동을 대상으로 하지 않으며, 아동의 개인정보를 알면서 수집하지 않습니다.

## 8. 방침 변경

이 방침이 바뀌면 이 페이지에 변경된 내용과 시행일을 게시합니다.

## 9. 문의

개인정보 처리에 관한 문의는 아래로 연락해 주세요.

**codebrunch27@gmail.com**

---

<sub>이 README와 `index.html`은 같은 내용을 담고 있습니다. 방침을 고칠 때는 **두 파일을 함께** 수정해 주세요.</sub>

---

<a name="english"></a>

# Link Keeper — Privacy Policy

**App:** 링크 보관함 (Link Keeper)
**Package:** `com.codebrunch.url`
**Effective date:** August 15, 2026
**Contact:** codebrunch27@gmail.com

## Summary

This app **does not collect personal information.** Everything you save stays on your device. Nothing is sent to the developer. The developer operates no server.

## 1. What the app stores

The following is stored **only on your device** and is never transmitted anywhere:

- Link addresses (URLs) you share or enter
- Titles, thumbnail URLs and favicon URLs read automatically from those web pages
- Memos you type
- Tags you create (name and colour)
- Bookmark state, read state, saved time
- App settings (save mode, thumbnail display, sort order, theme, retention period)
- A thumbnail image cache of up to 100 MB, pruned automatically

The app has **no account and no sign-in.** It does not collect your name, email, phone number, contacts, location, or device identifiers.

## 2. What the app does not do

- It does not send data to any server operated by the developer. **The developer operates no server.**
- It contains no analytics and no advertising SDKs.
- It does not track your activity.
- It does not sell or share any information with third parties.

## 3. When the app uses the internet

The app connects to the internet for **exactly one purpose**: when you save a link, it contacts **that website directly** to read its title and preview image.

Please note:

- The connection goes to **the website you saved**, not through any server of the developer.
- That website therefore receives **your IP address and a browser-like User-Agent string**, exactly as if you had opened the page in a browser yourself.
- Preview images are downloaded from the address the page specifies (usually that site or its CDN).
- How that website handles your information is governed by **its own privacy policy**, which the developer neither controls nor influences.

If there is no internet connection, only the address is saved and the preview is fetched later.

## 4. Backup

If **Android Auto Backup (Google Drive backup)** is enabled on your device, your saved links and settings may be included in a backup held in **your own Google account**.

- This is a Google feature; the developer cannot access its contents.
- You can turn it off under *Settings → System → Backup* on your device.
- Such backups are covered by the [Google Privacy Policy](https://policies.google.com/privacy).

## 5. Permissions

| Permission | Why |
|---|---|
| INTERNET | To fetch link titles and preview images |
| ACCESS_NETWORK_STATE | To fetch previews only when a connection is available |
| WAKE_LOCK, RECEIVE_BOOT_COMPLETED, FOREGROUND_SERVICE | Added automatically by WorkManager, the standard Android job-scheduling library, so preview fetching and cleanup of old links can run in the background |

The app does not request camera, location, contacts, or storage permissions.

## 6. Retention and deletion

- Saved links remain on your device until you delete them.
- You can delete links individually inside the app.
- You may set a **retention period** (1 week, 1 month, 6 months, 1 year) after which older links are deleted automatically. **Bookmarked links are never deleted automatically.**
- You can clear the image cache in Settings.
- **Uninstalling the app removes all of its data from the device.** (Google account backups, see section 4, are separate.)

Because the developer holds no user data, there is nothing for the developer to disclose, correct, or delete on request.

## 7. Children

This app is not directed at children and does not knowingly collect information from them.

## 8. Changes

If this policy changes, the updated text and its effective date will be posted on this page.

## 9. Contact

**codebrunch27@gmail.com**
