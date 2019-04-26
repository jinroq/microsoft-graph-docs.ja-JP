---
title: アクセス許可
description: '組織のアプリカタログ (テナントのアプリカタログ) からアプリを削除します。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 35a131309445f0a84bdc54690e1f88b5a0ad31f0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335232"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a>組織のアプリカタログからアプリを削除する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

組織のアプリカタログ (テナントのアプリカタログ) から[アプリ](../resources/teamsapp.md)を削除します。 組織のアプリカタログからアプリを削除するには、 `organization` teamsCatalogApp リソース**** で、を " [](../resources/teamsapp.md) " として指定します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。

>**注:** この API は、グローバル管理者のみが呼び出すことができます。 

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)|
|:----------------------------------     |:-------------|
| 委任 (職場または学校のアカウント)     | AppCatalog.ReadWrite.All |
| 委任 (個人用 Microsoft アカウント) | サポートされていません|
| アプリケーション                            | 非サポート|

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー        | 値           |
|:--------------|:--------------  |
| Authorization | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文

なし。

>**注:** の[発行済みアプリの一覧](./teamsapp-list.md)から返された ID を使用して、更新するアプリを参照します。 zip アプリパッケージのマニフェストからの ID は使用しないでください。

## <a name="response"></a>応答

```
HTTP/1.1 204 No Content
```

## <a name="example"></a>例

### <a name="request"></a>要求

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a>応答

```http
HTTP/1.1 204 No Content
```
