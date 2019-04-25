---
title: managedAppPolicy リソースの種類
description: ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 610012b216a0fe924af3cd4f08fb3928e504454b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573817"
---
# <a name="managedapppolicy-resource-type"></a>managedAppPolicy リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List managedAppPolicies](../api/intune-mam-managedapppolicy-list.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get managedAppPolicy](../api/intune-mam-managedapppolicy-get.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[targetApps アクション](../api/intune-mam-managedapppolicy-targetapps.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|ポリシーの表示名。|
|説明|String|ポリシーの説明。|
|createdDateTime|DateTimeOffset|ポリシーが作成された日時。|
|lastModifiedDateTime|DateTimeOffset|ポリシーが変更された最終日時。|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。|
|id|String|エンティティのキー。|
|version|String|エンティティのバージョン。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String"
}
```





