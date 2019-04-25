---
title: wipeManagedAppRegistrationByDeviceTag アクション
description: 指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 650ff602101cead593d39603beb0b361ac0421dc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526875"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a>wipeManagedAppRegistrationByDeviceTag アクション

> **重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。

## <a name="prerequisites"></a>前提条件

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)||
| &nbsp;&nbsp; **MAM** | DeviceManagementApps.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a>要求ヘッダー

|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文

要求本文で、パラメーターの JSON 表記を指定します。

次の表に、このアクションで使用できるパラメーターを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|deviceTag|String|デバイス タグ|

## <a name="response"></a>応答

成功した場合、このアクションは `204 No Content` 応答コードを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

以下は、要求の例です。

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

``` http
HTTP/1.1 204 No Content
```






