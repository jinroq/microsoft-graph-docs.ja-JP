---
title: Update androidForWorkSettings
description: androidForWorkSettings オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 658744008af023fc2ad419aedc7a369f1ffbcb9f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976744"
---
# <a name="update-androidforworksettings"></a>Update androidForWorkSettings

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) オブジェクトのプロパティを更新します。

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
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) オブジェクトの JSON 表記を指定します。

次の表に、[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) 作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|Android for Work の設定の識別子|
|bindStatus|[androidforwork bindstatus](../resources/intune-androidforwork-androidforworkbindstatus.md)|Google EMM API を使用して、テナントの状態をバインドします。 可能な値は、`notBound`、`bound`、`boundAndValidated`、`unbinding` です。|
|lastAppSyncDateTime|DateTimeOffset|アプリ同期の最終完了時刻|
|lastAppSyncStatus|[androidforwork syncstatus](../resources/intune-androidforwork-androidforworksyncstatus.md)|最後のアプリケーションの同期結果。 可能な値は `success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none` です。|
|ownerUserPrincipalName|String|エンタープライズを作成した所有者の UPN|
|ownerOrganizationName|String|Android for Work のオンボーディング時に使用される組織名|
|lastModifiedDateTime|DateTimeOffset|Android for Work の設定の最終変更時刻|
|enrollmentTarget|[androidForWorkEnrollmentTarget](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|Android for Work デバイス管理にデバイスを登録できるユーザーを示します。 可能な値は、`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions` です。|
|targetGroupIds|String コレクション|enrollmentTarget が「Targeted」に設定されている場合、どの AAD グループが Android for Work デバイス管理にデバイスを登録できるかを指定します。|
|deviceownermanagementenabled|Boolean|CloudDPC を使用した Android デバイス所有者の管理に、このアカウントが flighting になるかどうかを示します。|



## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidforwork settings](../resources/intune-androidforwork-androidforworksettings.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 568

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```




