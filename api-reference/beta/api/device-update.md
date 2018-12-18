---
title: デバイスを更新する
description: デバイスのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: df86581c1edb531e822204698486358fac29f106
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356561"
---
# <a name="update-device"></a>デバイスを更新する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

デバイスのプロパティを更新します。

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
| 名前       | 種類 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

要求本文で、更新する[デバイス](../resources/device.md) プロパティの値を指定します。 要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。 最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|accountEnabled|ブール値| アカウントが有効な場合は **true**。それ以外の場合は **false**。 |
|operatingSystem|文字列|デバイス上のオペレーティング システムの種類。|
|operatingSystemVersion|String|デバイス上のオペレーティング システムのバージョン|
|displayName|文字列|デバイスの表示名。|
|isCompliant|Boolean|デバイスがモバイル デバイス管理 (MDM) ポリシーに準拠している場合は **true**。それ以外の場合は **false**。 これはのみ、Intune は、デバイスの OS の種類のか、 [MDM アプリケーションを承認された](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)Windows OS のデバイスで更新できます。 |
|isManaged|Boolean|デバイスがモバイル デバイス管理 (MDM) アプリで管理されている場合は **true**。それ以外の場合は **false**。 これはのみ、Intune は、デバイスの OS の種類のか、 [MDM アプリケーションを承認された](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)Windows OS のデバイスで更新できます。 |

使用することができます、**デバイス**・ リソースは、[拡張機能](/graph/extensibility-overview)をサポートするため、`PATCH`を追加、更新、または既存の**デバイス**インスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/beta/devices/{id}
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

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
