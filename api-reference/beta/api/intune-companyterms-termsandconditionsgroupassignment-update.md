---
title: termsAndConditionsGroupAssignment の更新
description: termsAndConditionsGroupAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8468502b6fe4f3d51503d3240c45e0f28193bd9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150247"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="cd3d9-103">termsAndConditionsGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="cd3d9-103">Update termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="cd3d9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd3d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd3d9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cd3d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd3d9-106">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cd3d9-106">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd3d9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="cd3d9-107">Prerequisites</span></span>
<span data-ttu-id="cd3d9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd3d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cd3d9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cd3d9-110">Permission type</span></span>|<span data-ttu-id="cd3d9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cd3d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd3d9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cd3d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd3d9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd3d9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cd3d9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cd3d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd3d9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd3d9-115">Not supported.</span></span>|
|<span data-ttu-id="cd3d9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cd3d9-116">Application</span></span>|<span data-ttu-id="cd3d9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd3d9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd3d9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cd3d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="cd3d9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd3d9-119">Request headers</span></span>
|<span data-ttu-id="cd3d9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd3d9-120">Header</span></span>|<span data-ttu-id="cd3d9-121">値</span><span class="sxs-lookup"><span data-stu-id="cd3d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd3d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd3d9-122">Authorization</span></span>|<span data-ttu-id="cd3d9-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cd3d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd3d9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="cd3d9-124">Accept</span></span>|<span data-ttu-id="cd3d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd3d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd3d9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cd3d9-126">Request body</span></span>
<span data-ttu-id="cd3d9-127">要求本文で、 [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cd3d9-127">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="cd3d9-128">次の表に、 [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cd3d9-128">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="cd3d9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd3d9-129">Property</span></span>|<span data-ttu-id="cd3d9-130">型</span><span class="sxs-lookup"><span data-stu-id="cd3d9-130">Type</span></span>|<span data-ttu-id="cd3d9-131">説明</span><span class="sxs-lookup"><span data-stu-id="cd3d9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd3d9-132">id</span><span class="sxs-lookup"><span data-stu-id="cd3d9-132">id</span></span>|<span data-ttu-id="cd3d9-133">String</span><span class="sxs-lookup"><span data-stu-id="cd3d9-133">String</span></span>|<span data-ttu-id="cd3d9-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="cd3d9-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="cd3d9-135">targetgroupid</span><span class="sxs-lookup"><span data-stu-id="cd3d9-135">targetGroupId</span></span>|<span data-ttu-id="cd3d9-136">String</span><span class="sxs-lookup"><span data-stu-id="cd3d9-136">String</span></span>|<span data-ttu-id="cd3d9-137">T&C ポリシーが割り当てられているグループの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="cd3d9-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="cd3d9-138">応答</span><span class="sxs-lookup"><span data-stu-id="cd3d9-138">Response</span></span>
<span data-ttu-id="cd3d9-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cd3d9-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd3d9-140">例</span><span class="sxs-lookup"><span data-stu-id="cd3d9-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd3d9-141">要求</span><span class="sxs-lookup"><span data-stu-id="cd3d9-141">Request</span></span>
<span data-ttu-id="cd3d9-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cd3d9-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="cd3d9-143">応答</span><span class="sxs-lookup"><span data-stu-id="cd3d9-143">Response</span></span>
<span data-ttu-id="cd3d9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cd3d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 169

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
  "targetGroupId": "Target Group Id value"
}
```




