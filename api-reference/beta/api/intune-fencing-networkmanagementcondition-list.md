---
title: NetworkManagementConditions を一覧表示する
description: NetworkManagementCondition オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: df785e5f00f747d68a486bbf936670c5f328935d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355333"
---
# <a name="list-networkmanagementconditions"></a><span data-ttu-id="2d919-103">NetworkManagementConditions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2d919-103">List networkManagementConditions</span></span>

> <span data-ttu-id="2d919-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d919-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d919-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d919-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d919-106">[Networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2d919-106">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d919-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2d919-107">Prerequisites</span></span>
<span data-ttu-id="2d919-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d919-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d919-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2d919-110">Permission type</span></span>|<span data-ttu-id="2d919-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2d919-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d919-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2d919-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d919-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d919-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2d919-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2d919-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d919-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d919-115">Not supported.</span></span>|
|<span data-ttu-id="2d919-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2d919-116">Application</span></span>|<span data-ttu-id="2d919-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d919-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d919-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2d919-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="2d919-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d919-119">Request headers</span></span>
|<span data-ttu-id="2d919-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d919-120">Header</span></span>|<span data-ttu-id="2d919-121">値</span><span class="sxs-lookup"><span data-stu-id="2d919-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d919-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d919-122">Authorization</span></span>|<span data-ttu-id="2d919-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d919-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d919-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2d919-124">Accept</span></span>|<span data-ttu-id="2d919-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d919-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d919-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2d919-126">Request body</span></span>
<span data-ttu-id="2d919-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2d919-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d919-128">応答</span><span class="sxs-lookup"><span data-stu-id="2d919-128">Response</span></span>
<span data-ttu-id="2d919-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2d919-129">If successful, this method returns a `200 OK` response code and a collection of [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d919-130">例</span><span class="sxs-lookup"><span data-stu-id="2d919-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d919-131">要求</span><span class="sxs-lookup"><span data-stu-id="2d919-131">Request</span></span>
<span data-ttu-id="2d919-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2d919-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="2d919-133">応答</span><span class="sxs-lookup"><span data-stu-id="2d919-133">Response</span></span>
<span data-ttu-id="2d919-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2d919-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 511

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.networkManagementCondition",
      "id": "c2919b8f-9b8f-c291-8f9b-91c28f9b91c2",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```






