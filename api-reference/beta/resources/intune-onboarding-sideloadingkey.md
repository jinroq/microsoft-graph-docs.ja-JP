---
title: sideLoadingKey リソースの種類
description: SideLoadingKey エンティティは、Windows 8 とテナントのビジネス アプリケーションのインストールの行に 8.1 のデバイスに必要です。
ms.openlocfilehash: cac2360e2c50e64e1b421df4efaf53802d78558b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074090"
---
# <a name="sideloadingkey-resource-type"></a>sideLoadingKey リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

SideLoadingKey エンティティは、Windows 8 とテナントのビジネス アプリケーションのインストールの行に 8.1 のデバイスに必要です。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト sideLoadingKeies](../api/intune-onboarding-sideloadingkey-list.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)コレクション|[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティと関係を一覧表示します。|
|[SideLoadingKey を取得します。](../api/intune-onboarding-sideloadingkey-get.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティと関係を参照してください。|
|[SideLoadingKey を作成します。](../api/intune-onboarding-sideloadingkey-create.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|新しい[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトを作成します。|
|[SideLoadingKey を削除します。](../api/intune-onboarding-sideloadingkey-delete.md)|なし|の[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)を削除します。|
|[SideLoadingKey を更新します。](../api/intune-onboarding-sideloadingkey-update.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|側のキーの一意の id の読み込み|
|value|文字列|側の読み込みキー] の値は 5 列 5 行値、hiphens によって区切られています。|
|displayName|String|側の読み込みキー名、it プロフェッショナルの管理者に表示されます。|
|説明|String|側キーの読み込み中の説明は、it プロフェッショナルの管理者に表示されます.|
|totalActivation|Int32|側の読み込みキー合計のアクティブ化、it プロフェッショナルの管理者に表示されます。|
|lastUpdatedDateTime|String|側の読み込みキー最終更新日 it プロフェッショナルの管理者に表示されます。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sideLoadingKey"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "String (identifier)",
  "value": "String",
  "displayName": "String",
  "description": "String",
  "totalActivation": 1024,
  "lastUpdatedDateTime": "String"
}
```





