---
title: Permissions
description: '組織のアプリケーション カタログ (テナント アプリケーション カタログ) からアプリケーションを削除します。 '
ms.openlocfilehash: c3ee6433f38cfd52548af5ac27f3e3c9891af8d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074157"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a>組織のアプリケーションのカタログからアプリケーションを削除します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

組織のアプリケーション カタログ (テナント アプリケーション カタログ) から[アプリケーション](../resources/teamsapp.md)を削除します。 組織のアプリケーションのカタログからアプリケーションを削除するのには次のように指定します。 `organization` [teamsCatalogApp](../resources/teamsapp.md)リソースで**distributionMethod**とします。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。

>**注:** グローバル管理者だけでは、この API を呼び出すことができます。 

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

>**注:** 更新するにはアプリケーションを参照するための[リストには、アプリケーションが公開されて](./teamsapp-list.md)呼び出しから返された ID を使用します。 Zip アプリケーション パッケージのマニフェストの ID を使用しません。

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
