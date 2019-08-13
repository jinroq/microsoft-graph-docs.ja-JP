---
title: GroupPolicyPresentationDropdownLists のリスト
description: GroupPolicyPresentationDropdownList オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9e730ac6cd49e0836540486d0d58599c26eeecc4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357825"
---
# <a name="list-grouppolicypresentationdropdownlists"></a><span data-ttu-id="a8edc-103">GroupPolicyPresentationDropdownLists のリスト</span><span class="sxs-lookup"><span data-stu-id="a8edc-103">List groupPolicyPresentationDropdownLists</span></span>

> <span data-ttu-id="a8edc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8edc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8edc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8edc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8edc-106">[Grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a8edc-106">List properties and relationships of the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8edc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a8edc-107">Prerequisites</span></span>
<span data-ttu-id="a8edc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8edc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8edc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a8edc-110">Permission type</span></span>|<span data-ttu-id="a8edc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a8edc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8edc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a8edc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8edc-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8edc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a8edc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a8edc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8edc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8edc-115">Not supported.</span></span>|
|<span data-ttu-id="a8edc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a8edc-116">Application</span></span>|<span data-ttu-id="a8edc-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8edc-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8edc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a8edc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="a8edc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8edc-119">Request headers</span></span>
|<span data-ttu-id="a8edc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8edc-120">Header</span></span>|<span data-ttu-id="a8edc-121">値</span><span class="sxs-lookup"><span data-stu-id="a8edc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8edc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8edc-122">Authorization</span></span>|<span data-ttu-id="a8edc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8edc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8edc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a8edc-124">Accept</span></span>|<span data-ttu-id="a8edc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a8edc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8edc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a8edc-126">Request body</span></span>
<span data-ttu-id="a8edc-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a8edc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8edc-128">応答</span><span class="sxs-lookup"><span data-stu-id="a8edc-128">Response</span></span>
<span data-ttu-id="a8edc-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a8edc-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8edc-130">例</span><span class="sxs-lookup"><span data-stu-id="a8edc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8edc-131">要求</span><span class="sxs-lookup"><span data-stu-id="a8edc-131">Request</span></span>
<span data-ttu-id="a8edc-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a8edc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="a8edc-133">応答</span><span class="sxs-lookup"><span data-stu-id="a8edc-133">Response</span></span>
<span data-ttu-id="a8edc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a8edc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 703

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
      "label": "Label value",
      "id": "ba3ff7c9-f7c9-ba3f-c9f7-3fbac9f73fba",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "defaultItem": {
        "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
        "displayName": "Display Name value",
        "value": "Value value"
      },
      "items": [
        {
          "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
          "displayName": "Display Name value",
          "value": "Value value"
        }
      ],
      "required": true
    }
  ]
}
```






