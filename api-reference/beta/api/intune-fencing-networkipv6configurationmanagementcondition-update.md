---
title: NetworkIPv6ConfigurationManagementCondition を更新します。
description: NetworkIPv6ConfigurationManagementCondition オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 10014f1ddde4914b97f52e92901266e06ae07c99
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357317"
---
# <a name="update-networkipv6configurationmanagementcondition"></a>NetworkIPv6ConfigurationManagementCondition を更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[NetworkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトのプロパティを更新します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementConfiguration.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトの JSON の形式を指定します。

[NetworkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)を作成するときに必要なプロパティを次の表に示します。

|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|管理条件の一意の識別子です。 システムでは、作成時に割り当てられた値が生成されます。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|一意な名前|String|管理条件の一意の名前です。 管理条件式で使用されます。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|displayName|String|管理者は、管理の条件の名前を定義します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|説明|String|管理者は、管理状態の説明を定義します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|createdDateTime|DateTimeOffset|管理条件が作成された時刻。 サービス側が生成されます。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|変更された日時|DateTimeOffset|管理条件が最後に修正された時間です。 サービス側を更新します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|eTag|String|管理条件の ETag。 サービス側を更新します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件に該当するプラットフォームです。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されます。 可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile` です。|
|ipV6Prefix|String|接続されている IPv6 サブネットです。 例: 2001:db8::/32|
|ipV6Gateway|String|IPv6 ゲートウェイ アドレスです。 例: 2001:db8::1|
|ipV6DNSServerList|String コレクション|アダプター用に構成された IPv6 の DNS サーバーをします。|
|dnsSuffixList|String コレクション|現在のネットワークの有効な DNS サフィックスです。 例: seattle.contoso.com|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 401

{
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "25811206-1206-2581-0612-812506128125",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```





