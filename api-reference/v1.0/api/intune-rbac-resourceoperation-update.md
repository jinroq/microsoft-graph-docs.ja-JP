---
title: resourceOperation の更新
description: resourceOperation オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23e822502a8ba64466fd3630eda2acb19bf044f2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251112"
---
# <a name="update-resourceoperation"></a>resourceOperation の更新

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementRBAC.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトの JSON 表記を指定します。

次の表に、[resourceOperation](../resources/intune-rbac-resourceoperation.md) の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|リソース操作のキー。 読み取り専用で、自動生成されます。|
|resourceName|String|この操作が実行されるリソースの名前。|
|actionName|String|この操作が実行するアクションの種類。 actionName は簡潔で、できるだけ少ない単語にする必要があります。|
|説明|String|リソース操作の説明。 Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。|



## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、更新された [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを応答本文で返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 227

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```



