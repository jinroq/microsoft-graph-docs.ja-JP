---
title: windowsAssignedAccessProfile リソースの種類
description: Windows のアクセスのプロファイルを割り当てられています。
author: tfitzmac
ms.openlocfilehash: 6b01f362c31f6e2791a00d8ff02a7ecd5b798e3c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328792"
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

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|profilename プロパティ|String|これは、[スタート] メニューの [このプレゼンテーションの構成が割り当てられているユーザーにこれらのアプリケーションのレイアウト、アプリケーションのグループを識別するために使用するフレンドリ名です。|
|showTaskBar|ブール型|この設定では、タスク バーを表示するかどうかを指定するのには管理ができます。|
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





