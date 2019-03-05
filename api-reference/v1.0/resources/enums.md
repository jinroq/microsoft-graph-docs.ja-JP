---
title: 列挙値
description: Microsoft Graph 列挙値。
localization_priority: Normal
ms.openlocfilehash: 86dcbb1fbbdc61a0855f45a6675efc80f4855010
ms.sourcegitcommit: 159cf5aaa39d3721d96d3fd800f6a8b91159f74d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2019
ms.locfileid: "30379515"
---
### <a name="contactrelationship-values"></a>contactrelationship 値

|メンバー|値|説明|
|:---|:---|:---|
|親行|.0|ユーザーの親。|
|合わせる|1-d| ユーザーの相対パス。|
|aide|pbm-2| ユーザーの aide。|
|診察|1/3| ユーザーの医師。|
|守護|2/4| ユーザーのガーディアン。|
|子供|5| ユーザーの子。|
|も|シックス| ユーザーとの特定されていない関係。|
|unknownfuturevalue という|7| 将来の互換性のためのマーカー値。|

### <a name="timezonestandard-values"></a>timeZoneStandard の値

| 値
|:-----------------
| ws
| iana


### <a name="freebusystatus-values"></a>freeBusyStatus の値

| メンバー            |値
|:------------------|:-------
| 増やし              | .0
| 一時的         | 1-d
| 多忙              | pbm-2
| oof               | 1/3
| workingElsewhere  | 2/4
| 不明           | -1


### <a name="attendeetype-values"></a>attendeeType の値

| 値
|:-------------------------
| 必須
| 省略可能
| resource


### <a name="externalaudiencescope-values"></a>externalaudiencescope 値

| 値
|:-------------------------
| none
| contactsOnly
| all


### <a name="automaticrepliesstatus-values"></a>automaticRepliesStatus の値

| 値
|:-------------------------
| 党
| alwaysEnabled
| スケジュール済み


### <a name="calendarcolor-values"></a>calendarcolor 値

| メンバー     | 値
|:-----------|:----------
| 自動       | -1
| ライトブルー  | .0
| ライトグリーン | 1-d
| ライトオレンジ| pbm-2
| ライトグレー  | 1/3
| ライト黄| 2/4
| ライト青緑  | 5
| ライトピンク  | シックス
| ライトブラウン | 7
| ライトレッド   | ~
| maxcolor   | i-9


### <a name="educationexternalsource-values"></a>educationExternalSource の値

| 値
|:-------------------------
| sis
| 手動
| unknownfuturevalue という


### <a name="educationgender-values"></a>educationGender の値

| 値
|:-------------------------
| female
| 男
| も
| unknownfuturevalue という


### <a name="eventtype-values"></a>eventType 値

| 値
|:-------------------------
| 単一インスタンス
| 発生
| 例外
| 連続マスター


### <a name="sensitivity-values"></a>感度の値

| 値
|:-------------------------
| 標準
| personal
| 機密性
| 機密


### <a name="importance-values"></a>重要度の値

| 値
|:-------------------------
| 低さ
| 標準
| 高額


### <a name="educationuserrole-values"></a>educationUserRole の値
| 値
|:---------------------
| student
| teacher
| none
| unknownfuturevalue という


### <a name="meetingmessagetype-values"></a>会議の messagetype の値

| 値
|:-----------------
| none
| meetingRequest
| 中止
| 承諾
| meetingTenativelyAccepted
| 辞退


### <a name="followupflagstatus-values"></a>の値

| 値
|:-------------------------
| notflagged 付き
| complete
| 示さ


### <a name="inferenceclassificationtype-values"></a>inferenceClassificationType の値

| 値
|:-----------------
| 注力
| も


### <a name="iosnotificationalerttype-values"></a>iosnotificationalerttype の値

| 値
|:-------------------------
| devicedefault
| 尺
| modal
| none

### <a name="deviceenrollmentfailurereason-values"></a>deviceEnrollmentFailureReason の値

| 値
|:-------------
| 不明
| 認証
| 承認
| accountvalidation
| uservalidation
| devicenotsupported
| inmaintenance
| badrequest
| featureNotSupported
| enrollmentRestrictionsEnforced
| clientdisconnected


### <a name="bodytype-values"></a>bodytype の値
| 値
|:---------
| text
| html


### <a name="locationtype-values"></a>locationType の値

| 値
|:-------------------------
| 既定値です。
| conferenceRoom
| homeAddress
| businessAddress
| geoCoordinates
| streetAddress
| ホテル
| レストラン
| localbusiness
| PostalAddress

### <a name="locationuniqueidtype-values"></a>locationUniqueIdType の値

| 値
|:-------------------------
| 不明
| locationstore
| 名簿
| 機密性
| 地図


### <a name="messageactionflag-values"></a>messageactionflag の値

| 値
|:-------------------------
| any
| call
| 交換
| フォローアップ
| 注意
| 転送
| noResponseNecessary
| 読み込む
| 返信
| replyToAll
| 中


### <a name="onenoteuserrole-values"></a>onenoteUserRole の値

| メンバー      | 値
|:------------|:------------
| Owner       | .0
| Contributor (投稿者) | 1-d
| Reader      | pbm-2
| なし        | -1


### <a name="operationstatus-values"></a>operationstatus の値

| 値
|:-----------------
| NotStarted
| 実行中
| Completed
| Failed


### <a name="onenotepatchactiontype-values"></a>onenotePatchActionType の値

| 値
|:-------------------------
| 置換
| 追加
| 削除する
| Insert
| ド

### <a name="onenotepatchinsertposition-values"></a>onenotePatchInsertPosition の値

| 値
|:-------------------------
| After
| Before


### <a name="phonetype-values"></a>phoneType の値

| 値
|:-------------------------
| コール
| 出張
| 体
| も
| アシスタント
| ホーム fax
| businessfax
| otherFax
| 携帯
| オン


### <a name="plannerpreviewtype-values"></a>プランの種類の値

| 値
|:-------------------------
| 自動
| nopreview
| checklist
| 説明
| reference


### <a name="status-values"></a>状態の値

| 値
|:-----------------
| active
| まし
| deleted
| すべて
| unknownfuturevalue という


### <a name="weekindex-values"></a>weekIndex の値

| 値
|:-------------------------
| まずは
| 補助
| 種類
| つめの
| 前の


### <a name="dayofweek-values"></a>dayOfWeek 値

| 値
|:-------------------------
| n
| 曜日
| 毎週
| 毎週
| 火曜日
| 金曜日
| 土日

### <a name="recurrencepatterntype-values"></a>recurrencePatternType の値

| 値
|:-------------------------
| 定期的
| あたり
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>recurrenceRangeType の値

| 値
|:-------------------------
| endDate
| 無制限
| 振ら


### <a name="onenotesourceservice-values"></a>onenoteSourceService の値
| 値
|:---------------------
| 不明
| OneDrive
| onedrive forbusiness
| onpremonedrive forbusiness


### <a name="responsetype-values"></a>responsetype の値

| 値
|:-------------------------
| none
| organizer
| tentativelyAccepted
| accepted
| 同意
| notresponded


### <a name="activitydomain-values"></a>activitydomain の値

| 値
|:-------------------------
| 不明
| 作業
| personal
| Unrestricted


### <a name="websitetype-values"></a>websitetype の値

| 値
|:-------------------------
| も
| コール
| 作業
| ブログ
| profile


### <a name="categorycolor-values"></a>カテゴリの色の値

| メンバー   |値    
|:---------|:--------
| none     | -1      
| preset0  | .0       
| preset1  | 1-d       
| preset2  | pbm-2       
| preset3  | 1/3       
| preset4  | 2/4       
| preset5  | 5       
| preset6  | シックス       
| preset7  | 7       
| preset8  | ~       
| preset9  | i-9       
| preset10 | 個      
| preset11 | #      
| preset12 | 個      
| preset13 | スリー      
| preset14 | 第      
| preset15 | 約      
| preset16 | 16      
| preset17 | インチ      
| preset18 | 個      
| preset19 | 年      
| preset20 | 1280      
| preset21 | 21      
| preset22 | ×      
| preset23 | 最高      
| preset24 | ソケット      

### <a name="alertfeedback-values"></a>alertfeedback 値

アナリストによって提供される警告での可能なフィードバック値。

|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|わかり.|
|truePositive|1-d|Alert は true-正の数値です。|
|falsePositive|pbm-2| 警告は誤検知です-正数。|
|benignPositive|1/3| 通知は害のない-正。|

### <a name="filehashtype-values"></a>filehashtype の値

ファイルハッシュの種類の列挙。

|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|不明な種類です。|
|sha1|1-d|SHA1 ハッシュの種類。|
|sha256|pbm-2| SHA256 ハッシュの種類。|
|md5|1/3| MD5 ハッシュ型。|
|authenticodeHash256|2/4| AuthenticodeHash256 ハッシュの種類。|
|lsHash|5| LsHash ハッシュの種類。|
|ctph|シックス| ctph ハッシュの種類。|
|peSha1|7| PESHA1 ハッシュの種類。|
|peSha256|~| PESHA256 ハッシュの種類。|

### <a name="connectiondirection-values"></a>connectiondirection 値

ネットワーク接続の方向を示す列挙 (受信/送信)。

|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|不明な接続。|
|受信|1-d|受信接続。|
|向き|pbm-2| 送信接続。|

### <a name="connectionstatus-values"></a>connectionstatus の値

接続の状態を列挙します。

|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|接続状態が不明です。|
|しよう|1-d|接続を試行しました。|
|失敗|pbm-2| 接続に成功しました。|
|ブロック|1/3| 接続がブロックされました。|
|フェール|2/4| 接続に失敗しました。|

### <a name="processintegritylevel-values"></a>processIntegrityLevel の値

プロセスの可能な整合性レベルの値。

|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|わかり.|
|ない|個|整合性レベルは信頼されていません。|
|低さ|1280| 整合性レベルは低くなっています。|
|medium|31| 整合性レベルは中程度です。|
|高額|40| 整合性レベルは High です。|
|system|50| 整合性レベルはシステムです。|

### <a name="registryhive-values"></a>registryhive 値

で[https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives)定義されているレジストリハイブの列挙。

|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|不明なハイブです。|
|currentconfig|1-d|HKEY_CURRENT_CONFIG ハイブ。|
|currentUser|pbm-2| HKEY_CURRENT_USER ハイブ。|
|localmachinesam|1/3| HKEY_LOCAL_MACHINE\SAM ハイブ。|
|localmachinesamsoftware|2/4| HKEY_LOCAL_MACHINE\Software ハイブ。|
|localMachineSystem|5| HKEY_LOCAL_MACHINE\System ハイブ。|
|ユーザー既定|シックス| HKEY_USERS\\既定のハイブ。|

### <a name="registryoperation-values"></a>registryoperation の値

レジストリキー名と値の一方または両方を変更した操作。

|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|不明なレジストリ値の種類です。|
|create|1-d|レジストリを作成します。|
|modify|pbm-2|レジストリを変更します。|
|delete|1/3|レジストリを削除します。|

### <a name="registryvaluetype-values"></a>registryvaluetype 値

で[https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types)定義されているレジストリ値の種類の列挙。

|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|不明なレジストリ値の種類です。|
|バイナリ|1-d|REG_BINARY レジストリ値の種類。|
|dword|pbm-2| REG_DWORD のレジストリ値の種類。|
|dwordLittleEndian|1/3| REG_DWORD_LITTLE_ENDIAN レジストリ値の種類。|
|dて dbigエンディアン|2/4| REG_DWORD_BIG_ENDIAN レジストリ値の種類。|
|expandsz|5| REG_EXPAND_SZ レジストリ値の種類。|
|link|シックス| REG_LINK レジストリ値の種類。|
|multisz|7| REG_MULTI_SZ レジストリ値の種類。|
|none|~| REG_NONE レジストリ値の種類。|
|qword|i-9| REG_QWORD レジストリ値の種類。|
|qwordlittleEndian|個| REG_QWORD_LITTLE_ENDIAN レジストリ値の種類。|
|sz|#| REG_SZ レジストリ値の種類。|

### <a name="alertseverity-values"></a>alertseverity 値

通知の重要度を列挙します。

|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|重要度が不明です。|
|だけ|1-d|重要度は情報のみです。|
|低さ|pbm-2| 重要度は低くなります。|
|medium|1/3| 重要度は中程度です。|
|高額|2/4| 重要度は high です。|

### <a name="alertstatus-values"></a>alertstatus の値

アラートライフサイクル状態 (ステージ) の可能な値。

|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|状態が不明です。|
|newalert|個| 通知は新規です。|
|inProgress|1280|通知が進行中です。|
|解析|31|アラートが解決されます。|

### <a name="emailrole-values"></a>emailrole 値
電子メールの役割に指定できる値。

|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|不明な役割。|
|sender|1-d|電子メールの送信者。|
|recipient|pbm-2|電子メールの受信者。|

### <a name="logontype-values"></a>logontype の値

ユーザーのサインイン方法に指定できる値。

|メンバー|値|説明|
|:---|:---|:---|
|不明|-1|わかり.|
|対話的|.0|ログオンは対話的です。|
|remoteinteractive|1-d| ログオンはリモート対話型です。|
|lan|pbm-2| ログオンはネットワークです。|
|batch|1/3| ログオンはバッチです。|
|service|2/4| ログオンはサービスです。|

### <a name="useraccountsecuritytype-values"></a>userAccountSecurityType の値

Windows 定義ごとに、ユーザーアカウントの種類 (グループメンバーシップ) に指定できる値。

|メンバー|値|説明|
|:---|:---|:---|
|不明|-1|わかり.|
|standard|.0|標準ユーザーグループのメンバ。|
|power|1-d| Power Users グループのメンバー。|
|者|pbm-2| Administrators グループのメンバー。|
