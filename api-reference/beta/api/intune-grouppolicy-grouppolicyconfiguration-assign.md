---
title: assign アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cddbaa0bd40f83b7a9a5160f55dc4a4d2fa750c5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990079"
---
# <a name="assign-action"></a><span data-ttu-id="fc8ae-103">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="fc8ae-103">assign action</span></span>

> <span data-ttu-id="fc8ae-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc8ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc8ae-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fc8ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc8ae-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fc8ae-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc8ae-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="fc8ae-107">Prerequisites</span></span>
<span data-ttu-id="fc8ae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fc8ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc8ae-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fc8ae-110">Permission type</span></span>|<span data-ttu-id="fc8ae-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fc8ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc8ae-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fc8ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc8ae-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc8ae-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fc8ae-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fc8ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc8ae-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc8ae-115">Not supported.</span></span>|
|<span data-ttu-id="fc8ae-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fc8ae-116">Application</span></span>|<span data-ttu-id="fc8ae-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc8ae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc8ae-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fc8ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="fc8ae-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fc8ae-119">Request headers</span></span>
|<span data-ttu-id="fc8ae-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fc8ae-120">Header</span></span>|<span data-ttu-id="fc8ae-121">値</span><span class="sxs-lookup"><span data-stu-id="fc8ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc8ae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc8ae-122">Authorization</span></span>|<span data-ttu-id="fc8ae-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fc8ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc8ae-124">承諾</span><span class="sxs-lookup"><span data-stu-id="fc8ae-124">Accept</span></span>|<span data-ttu-id="fc8ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc8ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc8ae-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fc8ae-126">Request body</span></span>
<span data-ttu-id="fc8ae-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fc8ae-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fc8ae-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="fc8ae-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fc8ae-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc8ae-129">Property</span></span>|<span data-ttu-id="fc8ae-130">型</span><span class="sxs-lookup"><span data-stu-id="fc8ae-130">Type</span></span>|<span data-ttu-id="fc8ae-131">説明</span><span class="sxs-lookup"><span data-stu-id="fc8ae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc8ae-132">assignments</span><span class="sxs-lookup"><span data-stu-id="fc8ae-132">assignments</span></span>|<span data-ttu-id="fc8ae-133">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fc8ae-133">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="fc8ae-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fc8ae-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fc8ae-135">応答</span><span class="sxs-lookup"><span data-stu-id="fc8ae-135">Response</span></span>
<span data-ttu-id="fc8ae-136">成功した場合、このアクション`200 OK`は応答コードと、応答本文で[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fc8ae-136">If successful, this action returns a `200 OK` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc8ae-137">例</span><span class="sxs-lookup"><span data-stu-id="fc8ae-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc8ae-138">要求</span><span class="sxs-lookup"><span data-stu-id="fc8ae-138">Request</span></span>
<span data-ttu-id="fc8ae-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fc8ae-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign

Content-type: application/json
Content-length: 350

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="fc8ae-140">応答</span><span class="sxs-lookup"><span data-stu-id="fc8ae-140">Response</span></span>
<span data-ttu-id="fc8ae-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fc8ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





