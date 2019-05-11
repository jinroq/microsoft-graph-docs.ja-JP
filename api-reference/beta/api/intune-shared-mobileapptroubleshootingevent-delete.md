---
title: MobileAppTroubleshootingEvent の削除
description: 複数のワークフローをサポートする Microsoft Graph API for Intune の Delete mobileAppTroubleshootingEvent メソッドについて説明します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: c3dd3b3df2412c934bd6bba0ad0b3909f8f8ec31
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898603"
---
# <a name="delete-mobileapptroubleshootingevent"></a>MobileAppTroubleshootingEvent の削除

> **重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)を削除します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)||
|&nbsp;&nbsp; **デバイスの管理**|DeviceManagementManagedDevices.ReadWrite.All|
|&nbsp; &nbsp; **トラブルシューティング**|DeviceManagementManagedDevices.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッドは `204 No Content` 応答コードを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 204 No Content
```




