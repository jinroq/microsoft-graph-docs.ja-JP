---
title: notificationMessageTemplate の更新
description: notificationMessageTemplate オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ba404f8a0c738891a9791c3f0875ecc2d4d4d99
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994279"
---
# <a name="update-notificationmessagetemplate"></a>notificationMessageTemplate の更新

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementServiceConfig.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求の本文で、[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトの JSON 表記を指定します。

次の表に、[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。|
|displayName|String|通知メッセージ テンプレートの表示名。|
|defaultLocale|String|要求されたロケールが使用できないときにフォールバックする既定のロケール。|
|brandingOptions|[notificationTemplateBrandingOptions](../resources/intune-notification-notificationtemplatebrandingoptions.md)|メッセージ テンプレートのブランド化オプション。 ブランド化は、Intune 管理コンソールで定義されます。 可能な値は、`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation` です。|
|roleScopeTagIds|文字列コレクション|このエンティティインスタンスの範囲タグのリスト。|



## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 259

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





