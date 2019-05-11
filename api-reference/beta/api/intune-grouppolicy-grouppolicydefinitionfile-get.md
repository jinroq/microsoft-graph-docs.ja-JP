---
title: GroupPolicyDefinitionFile の取得
description: GroupPolicyDefinitionFile オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a29bfd41838c37b8e2a90638e3cd914b9de6791
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33905113"
---
# <a name="get-grouppolicydefinitionfile"></a><span data-ttu-id="ccabe-103">GroupPolicyDefinitionFile の取得</span><span class="sxs-lookup"><span data-stu-id="ccabe-103">Get groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="ccabe-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ccabe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccabe-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ccabe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccabe-106">[Grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ccabe-106">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccabe-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ccabe-107">Prerequisites</span></span>
<span data-ttu-id="ccabe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ccabe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccabe-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ccabe-110">Permission type</span></span>|<span data-ttu-id="ccabe-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ccabe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccabe-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ccabe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ccabe-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccabe-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ccabe-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ccabe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccabe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ccabe-115">Not supported.</span></span>|
|<span data-ttu-id="ccabe-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ccabe-116">Application</span></span>|<span data-ttu-id="ccabe-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ccabe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccabe-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ccabe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ccabe-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ccabe-119">Optional query parameters</span></span>
<span data-ttu-id="ccabe-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ccabe-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccabe-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ccabe-121">Request headers</span></span>
|<span data-ttu-id="ccabe-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ccabe-122">Header</span></span>|<span data-ttu-id="ccabe-123">値</span><span class="sxs-lookup"><span data-stu-id="ccabe-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccabe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccabe-124">Authorization</span></span>|<span data-ttu-id="ccabe-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ccabe-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccabe-126">承諾</span><span class="sxs-lookup"><span data-stu-id="ccabe-126">Accept</span></span>|<span data-ttu-id="ccabe-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ccabe-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccabe-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ccabe-128">Request body</span></span>
<span data-ttu-id="ccabe-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ccabe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccabe-130">応答</span><span class="sxs-lookup"><span data-stu-id="ccabe-130">Response</span></span>
<span data-ttu-id="ccabe-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ccabe-131">If successful, this method returns a `200 OK` response code and [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccabe-132">例</span><span class="sxs-lookup"><span data-stu-id="ccabe-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccabe-133">要求</span><span class="sxs-lookup"><span data-stu-id="ccabe-133">Request</span></span>
<span data-ttu-id="ccabe-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ccabe-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
```

### <a name="response"></a><span data-ttu-id="ccabe-135">応答</span><span class="sxs-lookup"><span data-stu-id="ccabe-135">Response</span></span>
<span data-ttu-id="ccabe-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ccabe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 479

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
    "displayName": "Display Name value",
    "description": "Description value",
    "languageCodes": [
      "Language Codes value"
    ],
    "targetPrefix": "Target Prefix value",
    "targetNamespace": "Target Namespace value",
    "policyType": "admxIngested",
    "id": "940aa2a1-a2a1-940a-a1a2-0a94a1a20a94",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```




