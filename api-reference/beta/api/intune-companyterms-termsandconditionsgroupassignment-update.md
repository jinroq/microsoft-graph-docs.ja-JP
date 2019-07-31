---
title: TermsAndConditionsGroupAssignment の更新
description: TermsAndConditionsGroupAssignment オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: df33de128db8b141015326429b8bc1c172fd23c4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958432"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="2e5a4-103">TermsAndConditionsGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="2e5a4-103">Update termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="2e5a4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e5a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e5a4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2e5a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e5a4-106">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2e5a4-106">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e5a4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2e5a4-107">Prerequisites</span></span>
<span data-ttu-id="2e5a4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e5a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e5a4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2e5a4-110">Permission type</span></span>|<span data-ttu-id="2e5a4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2e5a4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e5a4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2e5a4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e5a4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e5a4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2e5a4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2e5a4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e5a4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e5a4-115">Not supported.</span></span>|
|<span data-ttu-id="2e5a4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2e5a4-116">Application</span></span>|<span data-ttu-id="2e5a4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e5a4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e5a4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2e5a4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2e5a4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e5a4-119">Request headers</span></span>
|<span data-ttu-id="2e5a4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e5a4-120">Header</span></span>|<span data-ttu-id="2e5a4-121">値</span><span class="sxs-lookup"><span data-stu-id="2e5a4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e5a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e5a4-122">Authorization</span></span>|<span data-ttu-id="2e5a4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2e5a4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e5a4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2e5a4-124">Accept</span></span>|<span data-ttu-id="2e5a4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2e5a4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e5a4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2e5a4-126">Request body</span></span>
<span data-ttu-id="2e5a4-127">要求本文で、 [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2e5a4-127">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="2e5a4-128">次の表に、 [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2e5a4-128">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="2e5a4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e5a4-129">Property</span></span>|<span data-ttu-id="2e5a4-130">型</span><span class="sxs-lookup"><span data-stu-id="2e5a4-130">Type</span></span>|<span data-ttu-id="2e5a4-131">説明</span><span class="sxs-lookup"><span data-stu-id="2e5a4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e5a4-132">id</span><span class="sxs-lookup"><span data-stu-id="2e5a4-132">id</span></span>|<span data-ttu-id="2e5a4-133">String</span><span class="sxs-lookup"><span data-stu-id="2e5a4-133">String</span></span>|<span data-ttu-id="2e5a4-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="2e5a4-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="2e5a4-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="2e5a4-135">targetGroupId</span></span>|<span data-ttu-id="2e5a4-136">String</span><span class="sxs-lookup"><span data-stu-id="2e5a4-136">String</span></span>|<span data-ttu-id="2e5a4-137">T&C ポリシーが割り当てられているグループの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="2e5a4-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="2e5a4-138">応答</span><span class="sxs-lookup"><span data-stu-id="2e5a4-138">Response</span></span>
<span data-ttu-id="2e5a4-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2e5a4-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e5a4-140">例</span><span class="sxs-lookup"><span data-stu-id="2e5a4-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e5a4-141">要求</span><span class="sxs-lookup"><span data-stu-id="2e5a4-141">Request</span></span>
<span data-ttu-id="2e5a4-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2e5a4-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="2e5a4-143">応答</span><span class="sxs-lookup"><span data-stu-id="2e5a4-143">Response</span></span>
<span data-ttu-id="2e5a4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2e5a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





