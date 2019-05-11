---
title: enrollmentConfigurationAssignment の作成
description: 新しい enrollmentConfigurationAssignment オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16a316a0f6c06080c3962749242ed01073dc23f7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900048"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="e056e-103">enrollmentConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="e056e-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="e056e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e056e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e056e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e056e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e056e-106">新しい [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e056e-106">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e056e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e056e-107">Prerequisites</span></span>
<span data-ttu-id="e056e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e056e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e056e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e056e-110">Permission type</span></span>|<span data-ttu-id="e056e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e056e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e056e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e056e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e056e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e056e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e056e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e056e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e056e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e056e-115">Not supported.</span></span>|
|<span data-ttu-id="e056e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e056e-116">Application</span></span>|<span data-ttu-id="e056e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e056e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e056e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e056e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e056e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e056e-119">Request headers</span></span>
|<span data-ttu-id="e056e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e056e-120">Header</span></span>|<span data-ttu-id="e056e-121">値</span><span class="sxs-lookup"><span data-stu-id="e056e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e056e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e056e-122">Authorization</span></span>|<span data-ttu-id="e056e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e056e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e056e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e056e-124">Accept</span></span>|<span data-ttu-id="e056e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e056e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e056e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e056e-126">Request body</span></span>
<span data-ttu-id="e056e-127">要求本文で、enrollmentConfigurationAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e056e-127">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="e056e-128">次の表に、enrollmentConfigurationAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e056e-128">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="e056e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e056e-129">Property</span></span>|<span data-ttu-id="e056e-130">型</span><span class="sxs-lookup"><span data-stu-id="e056e-130">Type</span></span>|<span data-ttu-id="e056e-131">説明</span><span class="sxs-lookup"><span data-stu-id="e056e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e056e-132">id</span><span class="sxs-lookup"><span data-stu-id="e056e-132">id</span></span>|<span data-ttu-id="e056e-133">String</span><span class="sxs-lookup"><span data-stu-id="e056e-133">String</span></span>|<span data-ttu-id="e056e-134">登録構成の割り当てのキー</span><span class="sxs-lookup"><span data-stu-id="e056e-134">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="e056e-135">target</span><span class="sxs-lookup"><span data-stu-id="e056e-135">target</span></span>|[<span data-ttu-id="e056e-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e056e-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e056e-137">テナント内の管理されたデバイスへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="e056e-137">Represents an assignment to managed devices in the tenant</span></span>|



## <a name="response"></a><span data-ttu-id="e056e-138">応答</span><span class="sxs-lookup"><span data-stu-id="e056e-138">Response</span></span>
<span data-ttu-id="e056e-139">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e056e-139">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e056e-140">例</span><span class="sxs-lookup"><span data-stu-id="e056e-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e056e-141">要求</span><span class="sxs-lookup"><span data-stu-id="e056e-141">Request</span></span>
<span data-ttu-id="e056e-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e056e-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e056e-143">応答</span><span class="sxs-lookup"><span data-stu-id="e056e-143">Response</span></span>
<span data-ttu-id="e056e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e056e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




