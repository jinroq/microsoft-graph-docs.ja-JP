---
title: OneDrive ファイル ストレージ API の概要
description: OneDrive は、Office 365 のファイル ハブです。
ms.openlocfilehash: dcd16969a2f1b1f6898696fe0be9539d50800252
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092363"
---
# <a name="onedrive-file-storage-api-overview"></a>OneDrive ファイル ストレージ API の概要

OneDrive は、Office 365 のファイル ハブです。
ファイルは、Microsoft Teams、グループ、SharePoint など、さまざまなコンテキストで利用されています。
OneDrive によりユーザーは、保存場所に関係なくそれらのファイルにアクセスすることができ、Microsoft Graph を使用すれば、単一の API でそれを操作できます。

Office 365 のファイルは[ドライブ][Drive API]に保存されています。
ユーザーは、ファイルを個人的なドライブ - 自分の OneDrive - または [SharePoint][] ドキュメント ライブラリを利用した共有ドライブに保存できます。
OneDrive の柔軟性のおかげで、ユーザーは、それぞれにとって最適な方法で共同作業をすることができます。
ユーザーは、ファイルへのリンクを共有したり、ファイルをチーム ドライブにコピーまたは移動したり、Outlook で OneDrive ファイルをメール メッセージに添付したりすることができます。

## <a name="why-integrate-with-onedrive-file-storage-in-the-cloud"></a>OneDrive ファイル ストレージをクラウドに統合する理由

### <a name="tap-into-an-ecosystem-with-billions-of-files"></a>何十億ものファイルをエコシステムで管理する

OneDrive ユーザーは、任意のデバイスから、オンラインまたはオフラインでファイルにアクセスすることができ、組織内外の人とファイルを共有することができます
OneDrive を利用すれば、Word、Excel、PowerPoint などの慣れ親しんだアプリを使用してリアルタイムで共同作成できます。
Microsoft Graph によりファイルに対しては、何百種類もの形式の豊富なサムネイル、ビデオ ストリーミング、分析などの機能を利用できます。
OneDrive のデータは、ユーザーが信頼する方法で、高度な暗号化、コンプライアンス、およびセキュリティの機能によって保護されます。

OneDrive アプリは 5 億を超えるデバイスで実行されており、Fortune 500 企業の 85% 以上が OneDrive for Business を使用しています。アプリを OneDrive に統合することにより、すでにそこで日常的に作業を実行している何百万というユーザー、学生、およびビジネス ユーザーとつながって、彼らを関係付けることができます。

### <a name="store-your-apps-files-in-a-powerful-cloud"></a>アプリのファイルを強力なクラウドに保存する

ファイルを OneDrive に保存すると、アプリで Microsoft クラウドのさまざまな機能を利用することができ、ユーザーはどこからでも自分のファイルにアクセスすることができるようになります。
[ファイル ピッカー][] SDK を使用することにより、OneDrive のユーザーが慣れ親しんでいるのと同じエクスペリエンスを使用して、独自のアプリ内から、OneDrive 内のファイルを開いたり、ダウンロードしたり、保存したり、共有したりすることができます。
選択されたファイルに関する情報を、ファイル選択 SDK から直接取得したり、Microsoft Graph API を直接使用してファイルに関する深い対話操作を実行したりします。
[特殊フォルダー][]を使用して、`Documents` や `Camera Roll` など、OneDrive 上のよく知られた場所にファイルを保存したり、アプリに独自の個人用フォルダーを割り当てたりします。

### <a name="bring-your-app-straight-to-users-within-onedrive"></a>OneDrive 内からユーザーに対してアプリを直接立ち上げる

OneDrive を使用する顧客は、OneDrive 内から直接アプリを使用または立ち上げて、ファイルを開いたり、編集したり、プレビューしたりできます。
OneDrive の[ファイル ハンドラー][]拡張機能を使用することにより、独自のカスタム ファイル拡張子に対してアイコンやプレビュー機能を提供したり、アプリを **[新規]** ボタンに追加したり、独自のカスタム アクションをメニュー バーに追加してアプリが起動するようにしたりできます。

### <a name="work-with-content-in-formats-your-app-understands"></a>アプリの認識する形式でコンテンツを処理する

アプリは、最も都合の良い形式でファイルの内容を取得できます。
アプリでは、何百という異なるファイル形式のために、カスタム サイズの[サムネイル][]を表示できます。
PDF など、さまざまな代替[形式][]でファイルをダウンロードできます。
[プレビュー][] API (ベータ版) を使用することにより、OneDrive ファイルのプレビューをアプリ内に埋め込むこともできます。

### <a name="work-with-file-content-and-metadata-without-downloading-the-binary"></a>バイナリをダウンロードすることなくファイルの内容およびメタデータを処理する

Microsoft Graph を利用すれば、バイナリをダウンロードしなくても、REST API を通じて、豊かな内容にアクセスできます。
[写真][]、[オーディオ][]、および [ビデオ][]のファイルから抽出したメタデータを調べます。
[Excel API][] は、Excel ブックに保存されている生のデータを直接操作するために使用します。
[Notes API][] は、OneNote のノートブックの内容にアクセスするために使用します。

### <a name="react-to-file-changes"></a>ファイルへの変更に対応する

アプリは [webhooks][] によって、ファイルに変更が加えられた時点で通知を受け取り、それに短時間で対応することができます。
[delta API][] を使用することにより、アプリがクラウドと同期した最後の時点以降で、どのような変更が加えられたかを調べます。

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスをお探しですか?

- [Microsoft Graph v1.0 の OneDrive ファイル ストレージ API](/graph/api/resources/onedrive?view=graph-rest-1.0)
- [Microsoft Graph ベータ版の OneDrive ファイル ストレージ API](/graph/api/resources/onedrive?view=graph-rest-beta)

## <a name="next-steps"></a>次のステップ

Microsoft Graph v1.0 における [OneDrive API の使用][Drive API]に関する詳細を確認する。

[SharePoint]: sharepoint-concept-overview.md
[ファイル ピッカー]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[ファイル ハンドラー]: https://docs.microsoft.com/onedrive/developer/file-handlers
[特殊フォルダー]: /graph/api/drive-get-specialfolder?view=graph-rest-1.0
[メモ API]: integrate-with-onenote.md
[Excel API]: /graph/api/resources/excel?view=graph-rest-1.0
[REST API]: /graph/api/resources/onedrive?view=graph-rest-1.0
[delta API]: /graph/api/driveitem-delta?view=graph-rest-1.0
[ビデオ]: /graph/api/resources/video?view=graph-rest-1.0
[写真]: /graph/api/resources/photo?view=graph-rest-1.0
[オーディオ]: /graph/api/resources/audio?view=graph-rest-1.0
[形式]: /graph/api/driveitem-get-content-format?view=graph-rest-1.0
[サムネイル]: /graph/api/driveitem-list-thumbnails?view=graph-rest-1.0
[プレビュー]: /graph/api/driveitem-preview?view=graph-rest-beta
[webhooks]: /graph/api/resources/webhooks?view=graph-rest-1.0
[Drive API]: /graph/api/resources/onedrive?view=graph-rest-1.0
