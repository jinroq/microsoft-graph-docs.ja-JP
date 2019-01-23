---
title: user の作成
description: 新しいユーザー オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f8cf0fb067c5a9cac80308f49fe07af122c1b47
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392880"
---
# <a name="create-user"></a>user の作成

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい [user](../resources/intune-shared-user.md) オブジェクトを作成します。

## <a name="prerequisites"></a>前提条件

この API を呼び出すには次のアクセス許可のいずれかが必要です。 アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。  必要な特定のアクセス許可は、コンテキストに依存します。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)||
| &nbsp; &nbsp; **デバイスの管理** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp; **MAM** | DeviceManagementApps.ReadWrite.All|
| &nbsp;&nbsp; **契約時** | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp; &nbsp; **トラブルシューティング** | DeviceManagementManagedDevices.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a>要求ヘッダー

|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文

要求本文で、user オブジェクトの JSON 表記を指定します。

次の表に、user の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|ユーザーの一意識別子。|
|**採用**||
|deviceEnrollmentLimit|Int32|ユーザーが登録を許可されているデバイスの最大数。 使用できる値は 5 または 1000 です。|

要求本文のプロパティのサポートは、コンテキストによって異なります。

## <a name="response"></a>応答

成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [user](../resources/intune-shared-user.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

以下は、要求の例です。

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a>応答

以下は、応答の例です。 注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しから返されるプロパティは、コンテキストによって異なります。

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



