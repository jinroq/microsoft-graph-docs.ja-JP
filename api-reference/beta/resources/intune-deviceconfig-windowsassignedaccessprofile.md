---
title: windowsAssignedAccessProfile リソースの種類
description: Windows のアクセスのプロファイルを割り当てられています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 893e81e544286c6877b9443d96f610acb939e934
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972853"
---
# <a name="windowsassignedaccessprofile-resource-type"></a>windowsAssignedAccessProfile リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows のアクセスのプロファイルを割り当てられています。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsAssignedAccessProfiles](../api/intune-deviceconfig-windowsassignedaccessprofile-list.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)コレクション|[WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)オブジェクトのプロパティと関係を一覧表示します。|
|[WindowsAssignedAccessProfile を取得します。](../api/intune-deviceconfig-windowsassignedaccessprofile-get.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|[WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsAssignedAccessProfile を作成します。](../api/intune-deviceconfig-windowsassignedaccessprofile-create.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|新しい[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)オブジェクトを作成します。|
|[WindowsAssignedAccessProfile を削除します。](../api/intune-deviceconfig-windowsassignedaccessprofile-delete.md)|なし|の[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)を削除します。|
|[WindowsAssignedAccessProfile を更新します。](../api/intune-deviceconfig-windowsassignedaccessprofile-update.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|[WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|profilename プロパティ|String|これは、[スタート] メニューの [このプレゼンテーションの構成が割り当てられているユーザーにこれらのアプリケーションのレイアウト、アプリケーションのグループを識別するために使用するフレンドリ名です。|
|showTaskBar|Boolean|この設定では、タスク バーを表示するかどうかを指定するのには管理ができます。|
|appUserModelIds|String コレクション|これらは、[スタート] メニューから起動できる唯一の Windows ストア アプリです。|
|desktopAppPaths|String コレクション|これらは、[スタート] メニューで利用可能なデスクトップ アプリケーションのパスと、唯一のアプリケーション、ユーザーが起動できるようです。|
|ユーザー アカウント|String コレクション|この構成にキオスクがロックアウトされているユーザー アカウントです。|
|startMenuLayoutXml|Binary|開始の既定のレイアウトを変更するのには管理者は、ユーザーが変更できないようにします。レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。 XML は、バイナリ形式である必要があります。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAssignedAccessProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "showTaskBar": true,
  "appUserModelIds": [
    "String"
  ],
  "desktopAppPaths": [
    "String"
  ],
  "userAccounts": [
    "String"
  ],
  "startMenuLayoutXml": "binary"
}
```





