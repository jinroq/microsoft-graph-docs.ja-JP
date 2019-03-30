---
title: termsAndConditions の作成
description: 新しい termsAndConditions オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1863abdc31b75d243e569ac363e54215e131af4b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986188"
---
# <a name="create-termsandconditions"></a>termsAndConditions の作成

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトを作成します。

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
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文において、termsAndConditions オブジェクトの JSON 表記を指定します。

次の表に、termsAndConditions の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|T&C ポリシーの一意識別子。|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。|
|modifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。|
|displayName|String|T&C ポリシー用に管理者が提供した名前。 |
|description|String|管理者が提供した T&C ポリシーの説明。|
|title|String|管理者が提供した契約条件のタイトル。 ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。|
|bodyText|String|管理者が提供する契約条件の本文で、通常は条件そのものです。 ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。|
|acceptanceStatement|String|使用条件に関する、管理者指定の説明内容です。通常は、T&C ポリシーに定められた使用条件を受け入れることの意味を記載します。 ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。|
|version|Int32|条件の現行バージョンを示す整数。 管理者が条件を変更し、修正された T&C ポリシーをユーザーが再承諾するように求める場合に増分されます。|



## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 505

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```




