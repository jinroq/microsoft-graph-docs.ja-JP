---
title: enrollmentConfigurationAssignment の作成
description: 新しい enrollmentConfigurationAssignment オブジェクトを作成します。
ms.openlocfilehash: 844415cb5e1b2a7160fdf08a992ffbd472d8e70c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072141"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="cd9b7-103">enrollmentConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="cd9b7-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="cd9b7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cd9b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd9b7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd9b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd9b7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cd9b7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd9b7-107">新しい [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cd9b7-107">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd9b7-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="cd9b7-108">Prerequisites</span></span>
<span data-ttu-id="cd9b7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd9b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd9b7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cd9b7-111">Permission type</span></span>|<span data-ttu-id="cd9b7-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cd9b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd9b7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cd9b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cd9b7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd9b7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cd9b7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cd9b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd9b7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd9b7-116">Not supported.</span></span>|
|<span data-ttu-id="cd9b7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cd9b7-117">Application</span></span>|<span data-ttu-id="cd9b7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd9b7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd9b7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cd9b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="cd9b7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd9b7-120">Request headers</span></span>
|<span data-ttu-id="cd9b7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd9b7-121">Header</span></span>|<span data-ttu-id="cd9b7-122">値</span><span class="sxs-lookup"><span data-stu-id="cd9b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd9b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd9b7-123">Authorization</span></span>|<span data-ttu-id="cd9b7-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cd9b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd9b7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cd9b7-125">Accept</span></span>|<span data-ttu-id="cd9b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cd9b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd9b7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cd9b7-127">Request body</span></span>
<span data-ttu-id="cd9b7-128">要求本文で、enrollmentConfigurationAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cd9b7-128">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="cd9b7-129">次の表に、enrollmentConfigurationAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cd9b7-129">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="cd9b7-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd9b7-130">Property</span></span>|<span data-ttu-id="cd9b7-131">型</span><span class="sxs-lookup"><span data-stu-id="cd9b7-131">Type</span></span>|<span data-ttu-id="cd9b7-132">説明</span><span class="sxs-lookup"><span data-stu-id="cd9b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd9b7-133">id</span><span class="sxs-lookup"><span data-stu-id="cd9b7-133">id</span></span>|<span data-ttu-id="cd9b7-134">String</span><span class="sxs-lookup"><span data-stu-id="cd9b7-134">String</span></span>|<span data-ttu-id="cd9b7-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cd9b7-135">Not yet documented</span></span>|
|<span data-ttu-id="cd9b7-136">target</span><span class="sxs-lookup"><span data-stu-id="cd9b7-136">target</span></span>|[<span data-ttu-id="cd9b7-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cd9b7-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cd9b7-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cd9b7-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cd9b7-139">応答</span><span class="sxs-lookup"><span data-stu-id="cd9b7-139">Response</span></span>
<span data-ttu-id="cd9b7-140">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cd9b7-140">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd9b7-141">例</span><span class="sxs-lookup"><span data-stu-id="cd9b7-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd9b7-142">要求</span><span class="sxs-lookup"><span data-stu-id="cd9b7-142">Request</span></span>
<span data-ttu-id="cd9b7-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cd9b7-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="cd9b7-144">応答</span><span class="sxs-lookup"><span data-stu-id="cd9b7-144">Response</span></span>
<span data-ttu-id="cd9b7-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cd9b7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




