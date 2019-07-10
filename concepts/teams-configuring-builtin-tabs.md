---
title: Microsoft Teams の組み込みタブ タイプの構成
description: Microsoft Graph API を使用して Microsoft Teams タブを作成または構成する
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: afd06dcfbefdab71a72ea2b73ff12e84328d361e
ms.sourcegitcommit: 3b39005e7cb76f57460c9e85542d86e039b67c46
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/10/2019
ms.locfileid: "35607400"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a>Microsoft Teams の組み込みタブ タイプの構成

Microsoft Graph API を使用して Microsoft Teams タブを[作成](/graph/api/teamstab-add?view=graph-rest-beta)または[構成](/graph/api/teamstab-update?view=graph-rest-beta)するには、アプリの `teamsAppId` と、その種類のアプリ用に提供される `entityId`、`contentUrl`、`removeUrl`、`websiteUrl` について理解しておく必要があります。
この記事では、組み込みタブ タイプのこれらの値を取得する方法について説明します。

## <a name="custom-tabs"></a>カスタム タブ

Microsoft Graph を使用して、作成した[タブ プロバイダー](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview) と関連付けるタブを構成するには、アプリの[構成 UI が Microsoft Teams に提供する](https://docs.microsoft.com/en-us/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest) `entityId`、`contentUrl`、`removeUrl`、`websiteUrl` を識別し、同じ `entityId`、`contentUrl`、`removeUrl`、`websiteUrl` の値を Microsoft Graph に渡します。

`teamsAppId` は、[Microsoft Teams のアプリ マニフェスト スキーマ](https://docs.microsoft.com/en-us/microsoftteams/platform/resources/schema/manifest-schema)の `id` と同じです。

## <a name="website-tabs"></a>Web サイトのタブ

Web サイトのタブの場合、`teamsAppId` は `com.microsoft.teamspace.tab.web` です。 構成を次に示します。

| プロパティ   | 型        | 説明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Null                                                     |
| contentUrl | string      | Web サイトの URL                                       |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      | Web サイトの URL                                       |

## <a name="planner-tabs"></a>Planner のタブ

Planner のタブの場合、teamsAppId は `com.microsoft.teamspace.tab.planner` です。 構成を次に示します。

| プロパティ   | 型        | 説明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | プラン ID (GET /planner/plans/{id} で使用する ID)。                                              |
| contentUrl | string      | `https://tasks.office.com/{tenantName}/Home/PlannerFrame?page=7&planId={planId}`。ここで、{tenantName} はテナントの名前 (example.onmicrosoft.com など) で、{planId} はエンティティ ID と同じです。  |
| removeUrl  | string      | contentUrl と同じ値。    |
| websiteUrl | string      | contentUrl と同じ値。   |

Planner タブに表示される新しいプランを作成するには、「[plannerPlan の作成](/graph/api/planner-post-plans?view=graph-rest-beta)」を参照してください。

## <a name="microsoft-stream-tabs"></a>Microsoft Stream のタブ

Microsoft Stream のタブの場合、`teamsAppId` は `com.microsoftstream.embed.skypeteamstab` です。 構成は以下のとおりです。

| プロパティ   | 型        | 説明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Null                                                     |
| contentUrl | string      | `https://web.microsoftstream.com/embed/video/{id}?autoplay=false&showinfo=true&app=microsoftteams&l={locale}`。ここで、{id} は、ビデオ ストリームの ID です。 ストリームの {id} を見つけるには、ブラウザーでストリームを開いて、URL を調べます。形式は、`https://{domain}.microsoftstream.com/video/{id}` になります。  |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      | `https://web.microsoftstream.com/video/{id}`。ここで、{id} は、ビデオ ストリームの ID です。    |

## <a name="microsoft-forms-tabs"></a>Microsoft Forms のタブ

Microsoft Forms のタブの場合、`teamsAppId` は `81fef3a6-72aa-4648-a763-de824aeafb7d` です。
構成を次に示します。

| プロパティ   | 型        | 説明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | フォームの ID。  この値を定義し、Forms Web サイトのフォームに移動して、フォームの URL (`https://forms.office.com/Pages/DesignPage.aspx#FormId={formId}`) を見つけます。      |
| contentUrl | string      | `https://forms.office.com/Pages/TeamsDesignPage.aspx?Host=Teams&lang={locale}&groupId={groupId}&tid={tid}&teamsTheme={theme}&upn={upn}&fragment=FormId%3D{formId}`。ここで、{formId} はエンティティ ID と同じで、{locale}、{groupId}、{tid}、{upn} はリテラルです。   |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      |  `https://forms.office.com`    |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a>Word、Excel、PowerPoint、PDF のタブ

次の表は、各アプリの `teamsAppId` の一覧を示しています。

| アプリ   | teamsAppId | 種類 (拡張子)                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| Word | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| Excel | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| PowerPoint  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| PDF | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

構成を次に示します。

| プロパティ   | 型        | 説明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | ファイルの sourceDoc ID。 これは、SharePoint でファイルを開き、アドレス バーを見ると確認できます。URL に `sourcedoc=%7B{sourceDocId}%7D` 句があります。 これは、ドキュメントの SharePoint ドライブ項目の webUrl から派生させることもできます。 詳細については、「[GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta)」を参照してください。 |
| contentUrl | 文字列      | ファイルの URL (`{folder-webUrl}/{item-name}` 形式)。 {folder-webUrl} はファイルを含む SharePoint フォルダーの webUrl です。これは SharePoint でファイルを開いてアドレス バーを確認するか、[GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta) から webUrl プロパティを使用することで確認できます。 {item-name} はファイル名です (例: file.docx)。これは [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta) の `name` プロパティです。 |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      | Null                                       |

### <a name="example-create-a-configured-word-tab"></a>例: 構成された Word タブを作成する

次の例では、構成された Word タブを作成します。

```http
POST https://graph.microsoft.com/v1.0/teams/{team-id}/channels/{channel-id}/tabs
{
  "displayName": "word",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/com.microsoft.teamspace.tab.file.staticviewer.word",
  "configuration": {
     "entityId": "115A90F4-AC9C-4F79-9837-36D1EFB3BE08",
     "contentUrl": "https://m365x165177.sharepoint.com/sites/4NewCloneWithClonableParts/Shared%20Documents/General/Employee Handbook.docx",
     "removeUrl": null,
     "websiteUrl": null
  }
}
```

## <a name="wiki-tabs"></a>Wiki のタブ

Wiki のタブの場合、`teamsAppId` は `com.microsoft.teamspace.tab.wiki` です。
Wiki のタブは、Graph による構成をサポートしていません。
ただし、構成が必要なものはそれほど多くありません。構成されていない Wiki のタブで、最初のユーザーが **[セット アップ] タブ**を選択するだけで構成できます。

## <a name="document-library-tabs"></a>ドキュメント ライブラリのタブ

ドキュメント ライブラリのタブの場合、`teamsAppId` は `com.microsoft.teamspace.tab.files.sharepoint` です。 構成を次に示します。

| プロパティ   | 型        | 説明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | 空の文字列 ("")                                        |
| contentUrl | string      | ドキュメントライブラリのルートフォルダーの URL。 この URL を確認するには、ブラウザーで SharePoint フォルダーを開き、URL をコピーして、"/"/"/" を削除します。 |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      | Null                                                     |

### <a name="example-create-a-configured-document-library-tab"></a>例: 構成されたドキュメントライブラリタブを作成する

次の例では、構成された Word タブを作成します。

```http
POST https://graph.microsoft.com/v1.0/teams/{team-id}/channels/{channel-id}/tabs
{
    "displayName": "Document%20Library1",
    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/com.microsoft.teamspace.tab.files.sharepoint",
    "configuration": {
        "entityId": "",
        "contentUrl": "https://microsoft.sharepoint.com/teams/WWWtest/Shared%20Documents",
        "removeUrl": null,
        "websiteUrl": null
    }
}
```

## <a name="onenote-tabs"></a>OneNote のタブ

OneNote のタブの場合、`teamsAppId` は `0d820ecd-def2-4297-adad-78056cde7c78` です。 構成は以下のとおりです。

| プロパティ   | 型        | 説明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | `{randomGuid}_{notebookId}`。ここで、{randomGuid} は、生成する GUID です。                                      |
| contentUrl | string      | フォーム`https://www.onenote.com/teams/TabContent?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{groupId}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}`の URL。ここ`{notebookId}` `{oneNoteWebUrl}`で、は[GET/groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta)にあります。 スラッシュは、エスケープする必要があります。 {groupId}、{locale}、{tid} はリテラルです。 |
| removeUrl  | string      | フォーム`https://www.onenote.com/teams/TabRemove?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{groupId}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}`の URL。ここ`{notebookId}` `{oneNoteWebUrl}`で、は[GET/groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta)にあります。 スラッシュは、エスケープする必要があります。 {groupId}、{locale}、{tid} はリテラルです。 |
| websiteUrl | 文字列      | フォームの URL `https://www.onenote.com/teams/TabRedirect?redirectUrl={oneNoteWebUrl}`。ここで、`oneNoteWebUrl` は、[GET /groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta) で見つけることができます。 |

## <a name="power-bi-tabs"></a>Power BI のタブ

Power BI のタブの場合、`teamsAppId` は `com.microsoft.teamspace.tab.powerbi` です。
構成はサポートされていません。

## <a name="sharepoint-page-and-list-tabs"></a>SharePoint のページとリスト タブ

SharePoint のページとリスト タブの場合、`teamsAppId` は `2a527703-1f6f-4559-a332-d8a7d288cd88` です。
構成はサポートされていません。
タブを構成する必要がある場合は、Web サイトのタブの使用を検討してください。
