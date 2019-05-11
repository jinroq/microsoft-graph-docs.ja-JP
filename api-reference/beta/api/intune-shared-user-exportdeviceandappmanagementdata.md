---
title: exportDeviceAndAppManagementData 関数
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4eda08e5ed2f164de5cb262a515be4eec3bcbfc2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898116"
---
# <a name="exportdeviceandappmanagementdata-function"></a>exportDeviceAndAppManagementData 関数

> **重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="prerequisites"></a>前提条件

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)||
| &nbsp; &nbsp; **オンボーディング** | DeviceManagementServiceConfig.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a>要求ヘッダー

|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文

次の表に、この関数で使用できるパラメーターを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|skip|Int32|まだ文書化されていません|
|top|Int32|まだ文書化されていません|

## <a name="response"></a>応答

成功した場合、この関数`200 OK`は応答コードと、応答本文で[Deviceandappmanagementdata](../resources/intune-onboarding-deviceandappmanagementdata.md)を返します。

## <a name="example"></a>例

### <a name="request"></a>要求

以下は、要求の例です。

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 143

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementData",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```



