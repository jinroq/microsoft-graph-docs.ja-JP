---
title: termsAndConditionsAssignment の作成
description: 新しい termsAndConditionsAssignment オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 0a6cc4024487610fe4d243a2957d99a0522d800b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333335"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="f8b14-103">termsAndConditionsAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="f8b14-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="f8b14-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f8b14-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8b14-105">新しい [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f8b14-105">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8b14-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f8b14-106">Prerequisites</span></span>
<span data-ttu-id="f8b14-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8b14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8b14-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f8b14-109">Permission type</span></span>|<span data-ttu-id="f8b14-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f8b14-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8b14-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f8b14-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f8b14-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8b14-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f8b14-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f8b14-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8b14-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8b14-114">Not supported.</span></span>|
|<span data-ttu-id="f8b14-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f8b14-115">Application</span></span>|<span data-ttu-id="f8b14-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8b14-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8b14-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f8b14-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f8b14-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f8b14-118">Request headers</span></span>
|<span data-ttu-id="f8b14-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f8b14-119">Header</span></span>|<span data-ttu-id="f8b14-120">値</span><span class="sxs-lookup"><span data-stu-id="f8b14-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8b14-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8b14-121">Authorization</span></span>|<span data-ttu-id="f8b14-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f8b14-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8b14-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f8b14-123">Accept</span></span>|<span data-ttu-id="f8b14-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f8b14-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8b14-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f8b14-125">Request body</span></span>
<span data-ttu-id="f8b14-126">要求本文で、termsAndConditionsAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f8b14-126">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="f8b14-127">次の表に、termsAndConditionsAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f8b14-127">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="f8b14-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8b14-128">Property</span></span>|<span data-ttu-id="f8b14-129">種類</span><span class="sxs-lookup"><span data-stu-id="f8b14-129">Type</span></span>|<span data-ttu-id="f8b14-130">説明</span><span class="sxs-lookup"><span data-stu-id="f8b14-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8b14-131">ID</span><span class="sxs-lookup"><span data-stu-id="f8b14-131">id</span></span>|<span data-ttu-id="f8b14-132">String</span><span class="sxs-lookup"><span data-stu-id="f8b14-132">String</span></span>|<span data-ttu-id="f8b14-133">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="f8b14-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="f8b14-134">target</span><span class="sxs-lookup"><span data-stu-id="f8b14-134">target</span></span>|[<span data-ttu-id="f8b14-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f8b14-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f8b14-136">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="f8b14-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="f8b14-137">応答</span><span class="sxs-lookup"><span data-stu-id="f8b14-137">Response</span></span>
<span data-ttu-id="f8b14-138">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f8b14-138">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8b14-139">例</span><span class="sxs-lookup"><span data-stu-id="f8b14-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8b14-140">要求</span><span class="sxs-lookup"><span data-stu-id="f8b14-140">Request</span></span>
<span data-ttu-id="f8b14-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f8b14-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="f8b14-142">応答</span><span class="sxs-lookup"><span data-stu-id="f8b14-142">Response</span></span>
<span data-ttu-id="f8b14-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f8b14-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



