---
title: termsAndConditionsAssignment の作成
description: 新しい termsAndConditionsAssignment オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a5be3c312ee4084eabfb5676d2215f5b414a73cb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958614"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="080ae-103">termsAndConditionsAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="080ae-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="080ae-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="080ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="080ae-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="080ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="080ae-106">新しい [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="080ae-106">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="080ae-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="080ae-107">Prerequisites</span></span>
<span data-ttu-id="080ae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="080ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="080ae-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="080ae-110">Permission type</span></span>|<span data-ttu-id="080ae-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="080ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="080ae-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="080ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="080ae-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="080ae-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="080ae-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="080ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="080ae-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="080ae-115">Not supported.</span></span>|
|<span data-ttu-id="080ae-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="080ae-116">Application</span></span>|<span data-ttu-id="080ae-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="080ae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="080ae-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="080ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="080ae-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="080ae-119">Request headers</span></span>
|<span data-ttu-id="080ae-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="080ae-120">Header</span></span>|<span data-ttu-id="080ae-121">値</span><span class="sxs-lookup"><span data-stu-id="080ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="080ae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="080ae-122">Authorization</span></span>|<span data-ttu-id="080ae-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="080ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="080ae-124">承諾</span><span class="sxs-lookup"><span data-stu-id="080ae-124">Accept</span></span>|<span data-ttu-id="080ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="080ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="080ae-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="080ae-126">Request body</span></span>
<span data-ttu-id="080ae-127">要求本文で、termsAndConditionsAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="080ae-127">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="080ae-128">次の表に、termsAndConditionsAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="080ae-128">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="080ae-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="080ae-129">Property</span></span>|<span data-ttu-id="080ae-130">型</span><span class="sxs-lookup"><span data-stu-id="080ae-130">Type</span></span>|<span data-ttu-id="080ae-131">説明</span><span class="sxs-lookup"><span data-stu-id="080ae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="080ae-132">id</span><span class="sxs-lookup"><span data-stu-id="080ae-132">id</span></span>|<span data-ttu-id="080ae-133">String</span><span class="sxs-lookup"><span data-stu-id="080ae-133">String</span></span>|<span data-ttu-id="080ae-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="080ae-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="080ae-135">target</span><span class="sxs-lookup"><span data-stu-id="080ae-135">target</span></span>|[<span data-ttu-id="080ae-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="080ae-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="080ae-137">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="080ae-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="080ae-138">応答</span><span class="sxs-lookup"><span data-stu-id="080ae-138">Response</span></span>
<span data-ttu-id="080ae-139">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="080ae-139">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="080ae-140">例</span><span class="sxs-lookup"><span data-stu-id="080ae-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="080ae-141">要求</span><span class="sxs-lookup"><span data-stu-id="080ae-141">Request</span></span>
<span data-ttu-id="080ae-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="080ae-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="080ae-143">応答</span><span class="sxs-lookup"><span data-stu-id="080ae-143">Response</span></span>
<span data-ttu-id="080ae-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="080ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 217

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





