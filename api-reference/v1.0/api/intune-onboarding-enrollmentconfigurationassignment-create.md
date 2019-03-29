---
title: enrollmentConfigurationAssignment の作成
description: 新しい enrollmentConfigurationAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a999e3286881d3e736904ed9c8e722aa78d28204
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963612"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="103a3-103">enrollmentConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="103a3-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="103a3-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="103a3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="103a3-105">新しい [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="103a3-105">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="103a3-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="103a3-106">Prerequisites</span></span>
<span data-ttu-id="103a3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="103a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="103a3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="103a3-109">Permission type</span></span>|<span data-ttu-id="103a3-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="103a3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="103a3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="103a3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="103a3-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="103a3-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="103a3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="103a3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="103a3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="103a3-114">Not supported.</span></span>|
|<span data-ttu-id="103a3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="103a3-115">Application</span></span>|<span data-ttu-id="103a3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="103a3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="103a3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="103a3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="103a3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="103a3-118">Request headers</span></span>
|<span data-ttu-id="103a3-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="103a3-119">Header</span></span>|<span data-ttu-id="103a3-120">値</span><span class="sxs-lookup"><span data-stu-id="103a3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="103a3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="103a3-121">Authorization</span></span>|<span data-ttu-id="103a3-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="103a3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="103a3-123">承諾</span><span class="sxs-lookup"><span data-stu-id="103a3-123">Accept</span></span>|<span data-ttu-id="103a3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="103a3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="103a3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="103a3-125">Request body</span></span>
<span data-ttu-id="103a3-126">要求本文で、enrollmentConfigurationAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="103a3-126">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="103a3-127">次の表に、enrollmentConfigurationAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="103a3-127">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="103a3-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="103a3-128">Property</span></span>|<span data-ttu-id="103a3-129">型</span><span class="sxs-lookup"><span data-stu-id="103a3-129">Type</span></span>|<span data-ttu-id="103a3-130">説明</span><span class="sxs-lookup"><span data-stu-id="103a3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="103a3-131">id</span><span class="sxs-lookup"><span data-stu-id="103a3-131">id</span></span>|<span data-ttu-id="103a3-132">String</span><span class="sxs-lookup"><span data-stu-id="103a3-132">String</span></span>|<span data-ttu-id="103a3-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="103a3-133">Not yet documented</span></span>|
|<span data-ttu-id="103a3-134">target</span><span class="sxs-lookup"><span data-stu-id="103a3-134">target</span></span>|[<span data-ttu-id="103a3-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="103a3-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="103a3-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="103a3-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="103a3-137">応答</span><span class="sxs-lookup"><span data-stu-id="103a3-137">Response</span></span>
<span data-ttu-id="103a3-138">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="103a3-138">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="103a3-139">例</span><span class="sxs-lookup"><span data-stu-id="103a3-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="103a3-140">要求</span><span class="sxs-lookup"><span data-stu-id="103a3-140">Request</span></span>
<span data-ttu-id="103a3-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="103a3-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="103a3-142">応答</span><span class="sxs-lookup"><span data-stu-id="103a3-142">Response</span></span>
<span data-ttu-id="103a3-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="103a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



