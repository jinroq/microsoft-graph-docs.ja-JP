---
title: マイクロソフトのチームでの組み込みタブの種類を構成します。
description: 'チームは Microsoft のグラフの Api を使用してタブを作成したり、Microsoft の構成 '
ms.openlocfilehash: 2485e65ebac0c7201fe8b8210f8e4af9b9c8f164
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092409"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a>マイクロソフトのチームでの組み込みタブの種類を構成します。

[作成](/graph/api/teamstab-add?view=graph-rest-beta)または Microsoft グラフ Api を使用して、マイクロソフトのチーム] タブ[を構成する](/graph/api/teamstab-update?view=graph-rest-beta)、理解する必要があります、 `teamsAppId` 、アプリケーションのと、 `entityId`、 `contentUrl`、`removeUrl`と`websiteUrl`のアプリケーションの種類を提供します。
この資料では、組み込みタブの種類のこれらの値を取得する方法について説明します。

## <a name="custom-tabs"></a>カスタム タブ

Microsoft Graph を使用して、記述した[タブのプロバイダー](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview)に関連付けられているタブを構成する、識別、 `entityId`、 `contentUrl`、`removeUrl`と`websiteUrl`がアプリケーションの[UI を提供するマイクロソフトのチーム構成](https://docs.microsoft.com/en-us/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest)では、同じを渡すと`entityId`、 `contentUrl`、 `removeUrl`、および`websiteUrl`値をグラフにします。

`teamsAppId`と同じでは、`id`の[アプリケーションは、マイクロソフトのチームのスキーマをマニフェスト](https://docs.microsoft.com/en-us/microsoftteams/platform/resources/schema/manifest-schema)にします。

## <a name="website-tabs"></a>Web サイトのタブ

Web サイトのタブの`teamsAppId`、 `com.microsoft.teamspace.tab.web`。 構成を次に示します。

| プロパティ   | 型        | 説明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| エンティティ Id   | 文字列      | Null                                                     |
| contentUrl | 文字列      | Web サイトの URL                                       |
| removeUrl  | 文字列      | Null                                                     |
| websiteUrl | 文字列      | Web サイトの URL                                       |

## <a name="planner-tabs"></a>プランナーのタブ

プランナーのタブは、teamsAppId、 `com.microsoft.teamspace.tab.planner`。 構成を次に示します。

| プロパティ   | 型        | 説明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| エンティティ Id   | 文字列      | プラン ID (GET/planner プラン/{id} で使用する ID) です。                                              |
| contentUrl | 文字列      | `https://tasks.office.com/{tenantName}/Home/PlannerFrame?page=7&planId={planId}`、{tenantName} がテナント (example.onmicrosoft.com)、などの名前であり、{planId} は、エンティティの ID と同じです。  |
| removeUrl  | 文字列      | ContentUrl 値と同じです。    |
| websiteUrl | 文字列      | ContentUrl 値と同じです。   |

[計画] タブに表示する新しい計画を作成するには、 [plannerPlan の作成](/graph/api/planner-post-plans?view=graph-rest-beta)を参照してください。

## <a name="microsoft-stream-tabs"></a>Microsoft ストリームのタブ

Microsoft ストリームのタブの`teamsAppId`、 `com.microsoftstream.embed.skypeteamstab`。 構成を次に示します。

| プロパティ   | 型        | 説明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| エンティティ Id   | 文字列      | Null                                                     |
| contentUrl | 文字列      | `https://web.microsoftstream.com/embed/video/{id}?autoplay=false&showinfo=true&app=microsoftteams&l={locale}`、ビデオ ストリームの ID {id} であります。 {} の id、ストリームを検索するには、お使いのブラウザーにストリームを開くと URL を参照: フォームのことが`https://{domain}.microsoftstream.com/video/{id}`。  |
| removeUrl  | 文字列      | Null                                                     |
| websiteUrl | 文字列      | `https://web.microsoftstream.com/video/{id}`、ビデオ ストリームの ID {id} であります。    |

## <a name="microsoft-forms-tabs"></a>Microsoft フォームのタブ

Microsoft フォームのタブの`teamsAppId`、 `81fef3a6-72aa-4648-a763-de824aeafb7d`。
構成:

| プロパティ   | 型        | 説明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| エンティティ Id   | 文字列      | フォームの ID です。  この値を定義し、フォームの web サイトでフォームに移動し、フォームの URL を検索する`https://forms.office.com/Pages/DesignPage.aspx#FormId={formId}`。      |
| contentUrl | 文字列      | `https://forms.office.com/Pages/TeamsDesignPage.aspx?Host=Teams&lang={locale}&groupId={groupId}&tid={tid}&teamsTheme={theme}&upn={upn}&fragment=FormId%3D{formId}`、{} は、同じエンティティの ID とのロケール {} が {グループ Id}、{tid}、{upn} リテラルします。   |
| removeUrl  | 文字列      | Null                                                     |
| websiteUrl | 文字列      |  `https://forms.office.com`    |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a>Word、Excel、PowerPoint、および PDF のタブ

リストを次の表の`teamsAppId`の各アプリケーションです。

| App   | teamsAppId | 種類 (拡張子)                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| Word | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| Excel | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| PowerPoint  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| PDF | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

構成はサポートされていません。

## <a name="wiki-tabs"></a>Wiki タブ

Wiki のタブの`teamsAppId`、 `com.microsoft.teamspace.tab.wiki`。
Wiki のタブは、グラフでの構成をサポートしていません。
ただし、ことはそう多くありません、未構成の wiki] タブ **] タブの設定**を構成する] をクリックする最初のユーザーだけではニーズに - を構成するに注意してください。

## <a name="document-library-tabs"></a>ドキュメント ライブラリのタブ

ドキュメント ライブラリのタブで、 `teamsAppId` 、 `com.microsoft.teamspace.tab.files.sharepoint`。 構成はサポートされていません。

## <a name="onenote-tabs"></a>OneNote のタブ

OneNote のタブの`teamsAppId`、 `0d820ecd-def2-4297-adad-78056cde7c78`。 構成を次に示します。

| プロパティ   | 型        | 説明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| エンティティ Id   | 文字列      | `{randomGuid}_{notebookId}`、{randomGuid} は、GUID を生成する場所です。                                      |
| contentUrl | 文字列      | フォームの URL `https://www.onenote.com/teams/TabContent?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{sectionsUrl}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}`、 `{sectionsUrl}`、 `{notebookId}`、および`{oneNoteWebUrl}` [/groups/{id}/onenote ノートブックを取得](/graph/api/onenote-list-notebooks?view=graph-rest-beta)することにあります。 スラッシュをエスケープする必要があります。 {ロケール} と {tid} はリテラルです。 |
| removeUrl  | 文字列      | フォームの URL `https://www.onenote.com/teams/TabRemove?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{sectionsUrl}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}`、 `{sectionsUrl}`、 `{notebookId}`、および`{oneNoteWebUrl}` [/groups/{id}/onenote ノートブックを取得](/graph/api/onenote-list-notebooks?view=graph-rest-beta)することにあります。 スラッシュをエスケープする必要があります。 {ロケール} と {tid} はリテラルです。 |
| websiteUrl | 文字列      | フォームの URL `https://www.onenote.com/teams/TabRedirect?redirectUrl={oneNoteWebUrl}`、 `oneNoteWebUrl` [/groups/{id}/onenote ノートブックを取得する](/graph/api/onenote-list-notebooks?view=graph-rest-beta)を参照して |

## <a name="power-bi-tabs"></a>電源双タブ

電源 BI のタブの`teamsAppId`、 `com.microsoft.teamspace.tab.powerbi`。
構成はサポートされていません。

## <a name="sharepoint-page-and-list-tabs"></a>SharePoint ページおよび [リスト] タブ

SharePoint ページおよびリスト] タブでは、 `teamsAppId` 、 `2a527703-1f6f-4559-a332-d8a7d288cd88`。
構成はサポートされていません。
構成を使用する場合は、[web サイト] タブを使用して検討してください。
