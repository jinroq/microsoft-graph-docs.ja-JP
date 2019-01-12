---
title: デバイスを更新する
description: 登録済みデバイスのプロパティを更新します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f24372e122045eee9d79cde6334038f0dc1ccddf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962234"
---
# <a name="update-device"></a>デバイスを更新する

登録済みデバイスのプロパティを更新します。

承認済みモバイル デバイス管理 (MDM) アプリによって、デバイスの特定のプロパティのみを更新できます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.ReadWrite.All、Directory.AccessAsUser.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション | 非サポート |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> 注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

要求本文で、更新する[デバイス](../resources/device.md) プロパティの値を指定します。 要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。 最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|accountEnabled|ブール値| アカウントが有効な場合は **true**。それ以外の場合は **false**。 |
|operatingSystem|文字列|デバイス上のオペレーティング システムの種類。|
|operatingSystemVersion|String|デバイス上のオペレーティング システムのバージョン|
|displayName|文字列|デバイスの表示名。|
|isCompliant|Boolean|デバイスがモバイル デバイス管理 (MDM) ポリシーに準拠している場合は **true**。それ以外の場合は **false**。 これはのみ、Intune は、デバイスの OS の種類のか、 [MDM アプリケーションを承認された](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)Windows OS のデバイスで更新できます。 |
|isManaged|Boolean|デバイスがモバイル デバイス管理 (MDM) アプリで管理されている場合は **true**。それ以外の場合は **false**。 これはのみ、Intune は、デバイスの OS の種類のか、 [MDM アプリケーションを承認された](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)Windows OS のデバイスで更新できます。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
##### <a name="response"></a>応答

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
