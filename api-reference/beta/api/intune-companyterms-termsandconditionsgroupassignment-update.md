---
title: TermsAndConditionsGroupAssignment の更新
description: TermsAndConditionsGroupAssignment オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 21216e265c3af81fd0c53b76dda8f5015d13b10a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34971795"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="94e83-103">TermsAndConditionsGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="94e83-103">Update termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="94e83-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94e83-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94e83-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="94e83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94e83-106">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="94e83-106">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94e83-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="94e83-107">Prerequisites</span></span>
<span data-ttu-id="94e83-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94e83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94e83-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94e83-110">Permission type</span></span>|<span data-ttu-id="94e83-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="94e83-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94e83-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94e83-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94e83-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94e83-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="94e83-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94e83-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94e83-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94e83-115">Not supported.</span></span>|
|<span data-ttu-id="94e83-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94e83-116">Application</span></span>|<span data-ttu-id="94e83-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94e83-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94e83-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94e83-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="94e83-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94e83-119">Request headers</span></span>
|<span data-ttu-id="94e83-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94e83-120">Header</span></span>|<span data-ttu-id="94e83-121">値</span><span class="sxs-lookup"><span data-stu-id="94e83-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94e83-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94e83-122">Authorization</span></span>|<span data-ttu-id="94e83-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="94e83-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94e83-124">承諾</span><span class="sxs-lookup"><span data-stu-id="94e83-124">Accept</span></span>|<span data-ttu-id="94e83-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94e83-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94e83-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="94e83-126">Request body</span></span>
<span data-ttu-id="94e83-127">要求本文で、 [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="94e83-127">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="94e83-128">次の表に、 [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="94e83-128">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="94e83-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94e83-129">Property</span></span>|<span data-ttu-id="94e83-130">型</span><span class="sxs-lookup"><span data-stu-id="94e83-130">Type</span></span>|<span data-ttu-id="94e83-131">説明</span><span class="sxs-lookup"><span data-stu-id="94e83-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94e83-132">id</span><span class="sxs-lookup"><span data-stu-id="94e83-132">id</span></span>|<span data-ttu-id="94e83-133">String</span><span class="sxs-lookup"><span data-stu-id="94e83-133">String</span></span>|<span data-ttu-id="94e83-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="94e83-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="94e83-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="94e83-135">targetGroupId</span></span>|<span data-ttu-id="94e83-136">String</span><span class="sxs-lookup"><span data-stu-id="94e83-136">String</span></span>|<span data-ttu-id="94e83-137">T&C ポリシーが割り当てられているグループの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="94e83-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="94e83-138">応答</span><span class="sxs-lookup"><span data-stu-id="94e83-138">Response</span></span>
<span data-ttu-id="94e83-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="94e83-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94e83-140">例</span><span class="sxs-lookup"><span data-stu-id="94e83-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="94e83-141">要求</span><span class="sxs-lookup"><span data-stu-id="94e83-141">Request</span></span>
<span data-ttu-id="94e83-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94e83-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="94e83-143">応答</span><span class="sxs-lookup"><span data-stu-id="94e83-143">Response</span></span>
<span data-ttu-id="94e83-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="94e83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





