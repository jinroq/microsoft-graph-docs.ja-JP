---
title: userInstallStateSummary リソースの種類
description: ユーザーのインストール状態の要約のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 82782be90b0d9cda70def3a2e6d41ba1d76794a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955381"
---
# <a name="userinstallstatesummary-resource-type"></a>userInstallStateSummary リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ユーザーのインストール状態の要約のプロパティが含まれています。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[userInstallStateSummaries のリスト](../api/intune-books-userinstallstatesummary-list.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[userInstallStateSummary の取得](../api/intune-books-userinstallstatesummary-get.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[userInstallStateSummary の作成](../api/intune-books-userinstallstatesummary-create.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|新しい [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを作成します。|
|[userInstallStateSummary の削除](../api/intune-books-userinstallstatesummary-delete.md)|なし|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) を削除します。|
|[userInstallStateSummary の更新](../api/intune-books-userinstallstatesummary-update.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|userName|String|ユーザー名です。|
|installedDeviceCount|Int32|インストールされたデバイスの数です。|
|failedDeviceCount|Int32|失敗したデバイスの数です。|
|notInstalledDeviceCount|Int32|インストールされていないデバイスの数です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceStates|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション|電子ブックのインストールの状態です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userInstallStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "String (identifier)",
  "userName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```



