---
title: Contract リソースの種類
description: パートナーテナントと顧客テナントの間に存在する既存のパートナーシップを表します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0d8da7c20705796cdb612ad1a24c4d03ce160447
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341213"
---
# <a name="contract-resource-type"></a>Contract リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

パートナーテナントと顧客テナントの間に存在する既存のパートナーシップを表します。

> **重要:** パートナーテナントのみに存在します。 パートナーテナントは、microsoft の[クラウドソリューションプロバイダー](https://partnercenter.microsoft.com/en-us/partner/programs)、Office 365 シンジケート、または microsoft Advisor パートナープログラムの一部である microsoft パートナーに属する Azure AD テナントです。

## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[契約書を取得する](../api/contract-get.md) | 縮小 |特定の contract オブジェクトのプロパティを読み取ります。 |
|[契約書を一覧表示する](../api/contract-list.md) | Contract コレクション | パートナーテナント内の契約のリスト。 |

## <a name="properties"></a>プロパティ
| プロパティ   | 型 | 説明 |
|:---------------|:--------|:----------|
|contracttype|String|契約の種類。<br><br>使用可能な値は次のいずれかです。<br> *SyndicationPartner* -このお客様に対して O365 と Intune を排他的に resells して管理します。 これらのユーザーは、お客様を再販し、サポートしています。<br> *BreadthPartner* -パートナーは、このお客様に対して管理サポートを提供することができます。 ただし、パートナーはお客様に再販することは許可されていません。<br>*ResellerPartner* -シンジケートパートナーに似ていますが、パートナーがテナントへの排他的なアクセス権を持っていない点が異なります。 シンジケーションの場合、お客様は、Microsoft や他のパートナーから追加の直接サブスクリプションを購入することはできません。|
|id|Guid|このパートナーシップによって参照される顧客のテナントの一意識別子。 顧客テナントの組織リソースの id プロパティに対応します。 |
|defaultdomainname|String|顧客テナントの既定のドメイン名のコピー。 このコピーは、顧客とのパートナーシップが確立されたときに作成されます。 顧客のテナントの既定のドメイン名が変更されても、自動的には更新されません。|
|displayName|String|顧客のテナントの表示名のコピー。 このコピーは、顧客とのパートナーシップが確立されたときに作成されます。 顧客のテナントの表示名が変更されても、自動的には更新されません。|
|id|String| パートナーシップの一意識別子。 キー、読み取り専用 |

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Contract"
}-->

```json
{
  "contractType": "String",
  "customerId": "Guid",
  "defaultDomainName": "String",
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
