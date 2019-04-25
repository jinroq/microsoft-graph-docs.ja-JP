---
title: deviceCategory の更新
description: deviceCategory オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90f5305e2fb52b5ecd184aad837f2c9d8f6334ef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527113"
---
# <a name="update-devicecategory"></a>deviceCategory の更新

> **重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)||
| &nbsp;&nbsp; **デバイスの管理** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp; &nbsp; **オンボーディング** | DeviceManagementManagedDevices.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求

**デバイスの管理**

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

**オンボード**

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a>要求ヘッダー

|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文

要求本文で、[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトの JSON 表記を指定します。

次の表に、[deviceCategory](../resources/intune-shared-devicecategory.md) の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|デバイス カテゴリの一意識別子。 読み取り専用です。|
|**オンボーディング**|
|description|String|デバイス カテゴリに関するオプションの説明。|
|displayName|String|デバイス カテゴリの表示名。|

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

要求の例を次に示します。

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a>応答

以下は、応答の例です。 注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 応答プロパティは、状況に応じて異なります。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



