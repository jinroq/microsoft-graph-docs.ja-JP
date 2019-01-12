---
title: assign アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 455c51dee7f4e1a480fb28e965e0036f64149989
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938903"
---
# <a name="assign-action"></a><span data-ttu-id="dd2e6-103">assign アクション</span><span class="sxs-lookup"><span data-stu-id="dd2e6-103">assign action</span></span>

> <span data-ttu-id="dd2e6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dd2e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd2e6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd2e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd2e6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dd2e6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd2e6-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="dd2e6-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd2e6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="dd2e6-108">Prerequisites</span></span>
<span data-ttu-id="dd2e6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dd2e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd2e6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dd2e6-111">Permission type</span></span>|<span data-ttu-id="dd2e6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dd2e6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd2e6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dd2e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd2e6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd2e6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd2e6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dd2e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd2e6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd2e6-116">Not supported.</span></span>|
|<span data-ttu-id="dd2e6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dd2e6-117">Application</span></span>|<span data-ttu-id="dd2e6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd2e6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd2e6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dd2e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="dd2e6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dd2e6-120">Request headers</span></span>
|<span data-ttu-id="dd2e6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dd2e6-121">Header</span></span>|<span data-ttu-id="dd2e6-122">値</span><span class="sxs-lookup"><span data-stu-id="dd2e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd2e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd2e6-123">Authorization</span></span>|<span data-ttu-id="dd2e6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dd2e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd2e6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dd2e6-125">Accept</span></span>|<span data-ttu-id="dd2e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd2e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd2e6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="dd2e6-127">Request body</span></span>
<span data-ttu-id="dd2e6-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dd2e6-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dd2e6-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="dd2e6-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dd2e6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd2e6-130">Property</span></span>|<span data-ttu-id="dd2e6-131">型</span><span class="sxs-lookup"><span data-stu-id="dd2e6-131">Type</span></span>|<span data-ttu-id="dd2e6-132">説明</span><span class="sxs-lookup"><span data-stu-id="dd2e6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd2e6-133">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="dd2e6-133">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="dd2e6-134">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dd2e6-134">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="dd2e6-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="dd2e6-135">Not yet documented</span></span>|
|<span data-ttu-id="dd2e6-136">assignments</span><span class="sxs-lookup"><span data-stu-id="dd2e6-136">assignments</span></span>|<span data-ttu-id="dd2e6-137">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dd2e6-137">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="dd2e6-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="dd2e6-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dd2e6-139">応答</span><span class="sxs-lookup"><span data-stu-id="dd2e6-139">Response</span></span>
<span data-ttu-id="dd2e6-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="dd2e6-140">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd2e6-141">例</span><span class="sxs-lookup"><span data-stu-id="dd2e6-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd2e6-142">要求</span><span class="sxs-lookup"><span data-stu-id="dd2e6-142">Request</span></span>
<span data-ttu-id="dd2e6-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dd2e6-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 548

{
  "deviceConfigurationGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ],
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="dd2e6-144">応答</span><span class="sxs-lookup"><span data-stu-id="dd2e6-144">Response</span></span>
<span data-ttu-id="dd2e6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dd2e6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





