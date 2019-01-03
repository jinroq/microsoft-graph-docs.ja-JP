---
title: TermsAndConditionsGroupAssignment を作成します。
description: 新しい termsAndConditionsGroupAssignment オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 54bcf9591cbfc9cd9369e434b11440a8247ea813
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301387"
---
# <a name="create-termsandconditionsgroupassignment"></a><span data-ttu-id="c0e65-103">TermsAndConditionsGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="c0e65-103">Create termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="c0e65-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0e65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0e65-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0e65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0e65-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0e65-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0e65-107">新しい[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c0e65-107">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0e65-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c0e65-108">Prerequisites</span></span>
<span data-ttu-id="c0e65-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0e65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0e65-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0e65-111">Permission type</span></span>|<span data-ttu-id="c0e65-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0e65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0e65-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0e65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0e65-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0e65-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c0e65-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0e65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0e65-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0e65-116">Not supported.</span></span>|
|<span data-ttu-id="c0e65-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0e65-117">Application</span></span>|<span data-ttu-id="c0e65-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0e65-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0e65-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0e65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="c0e65-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0e65-120">Request headers</span></span>
|<span data-ttu-id="c0e65-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0e65-121">Header</span></span>|<span data-ttu-id="c0e65-122">値</span><span class="sxs-lookup"><span data-stu-id="c0e65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0e65-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0e65-123">Authorization</span></span>|<span data-ttu-id="c0e65-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c0e65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0e65-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c0e65-125">Accept</span></span>|<span data-ttu-id="c0e65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0e65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0e65-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0e65-127">Request body</span></span>
<span data-ttu-id="c0e65-128">要求の本文に termsAndConditionsGroupAssignment オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0e65-128">In the request body, supply a JSON representation for the termsAndConditionsGroupAssignment object.</span></span>

<span data-ttu-id="c0e65-129">次の表は、termsAndConditionsGroupAssignment を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c0e65-129">The following table shows the properties that are required when you create the termsAndConditionsGroupAssignment.</span></span>

|<span data-ttu-id="c0e65-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0e65-130">Property</span></span>|<span data-ttu-id="c0e65-131">種類</span><span class="sxs-lookup"><span data-stu-id="c0e65-131">Type</span></span>|<span data-ttu-id="c0e65-132">説明</span><span class="sxs-lookup"><span data-stu-id="c0e65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0e65-133">ID</span><span class="sxs-lookup"><span data-stu-id="c0e65-133">id</span></span>|<span data-ttu-id="c0e65-134">String</span><span class="sxs-lookup"><span data-stu-id="c0e65-134">String</span></span>|<span data-ttu-id="c0e65-135">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="c0e65-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="c0e65-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="c0e65-136">targetGroupId</span></span>|<span data-ttu-id="c0e65-137">String</span><span class="sxs-lookup"><span data-stu-id="c0e65-137">String</span></span>|<span data-ttu-id="c0e65-138">T & C のポリシーが割り当てられているグループの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="c0e65-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="c0e65-139">応答</span><span class="sxs-lookup"><span data-stu-id="c0e65-139">Response</span></span>
<span data-ttu-id="c0e65-140">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c0e65-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0e65-141">例</span><span class="sxs-lookup"><span data-stu-id="c0e65-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0e65-142">要求</span><span class="sxs-lookup"><span data-stu-id="c0e65-142">Request</span></span>
<span data-ttu-id="c0e65-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c0e65-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="c0e65-144">応答</span><span class="sxs-lookup"><span data-stu-id="c0e65-144">Response</span></span>
<span data-ttu-id="c0e65-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0e65-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 169

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
  "targetGroupId": "Target Group Id value"
}
```




