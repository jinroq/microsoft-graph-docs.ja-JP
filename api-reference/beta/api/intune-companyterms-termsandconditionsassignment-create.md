---
title: termsAndConditionsAssignment の作成
description: 新しい termsAndConditionsAssignment オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fe83995c1a0d7af5e3f0e2eea88813b7c490ba2a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398059"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="ce2f9-103">termsAndConditionsAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="ce2f9-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="ce2f9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ce2f9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce2f9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce2f9-107">新しい [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-107">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce2f9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ce2f9-108">Prerequisites</span></span>
<span data-ttu-id="ce2f9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ce2f9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce2f9-111">Permission type</span></span>|<span data-ttu-id="ce2f9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce2f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce2f9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce2f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce2f9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce2f9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ce2f9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce2f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce2f9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-116">Not supported.</span></span>|
|<span data-ttu-id="ce2f9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce2f9-117">Application</span></span>|<span data-ttu-id="ce2f9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce2f9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce2f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ce2f9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce2f9-120">Request headers</span></span>
|<span data-ttu-id="ce2f9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce2f9-121">Header</span></span>|<span data-ttu-id="ce2f9-122">値</span><span class="sxs-lookup"><span data-stu-id="ce2f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce2f9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce2f9-123">Authorization</span></span>|<span data-ttu-id="ce2f9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce2f9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ce2f9-125">Accept</span></span>|<span data-ttu-id="ce2f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce2f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce2f9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce2f9-127">Request body</span></span>
<span data-ttu-id="ce2f9-128">要求本文で、termsAndConditionsAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-128">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="ce2f9-129">次の表に、termsAndConditionsAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-129">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="ce2f9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce2f9-130">Property</span></span>|<span data-ttu-id="ce2f9-131">型</span><span class="sxs-lookup"><span data-stu-id="ce2f9-131">Type</span></span>|<span data-ttu-id="ce2f9-132">説明</span><span class="sxs-lookup"><span data-stu-id="ce2f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce2f9-133">id</span><span class="sxs-lookup"><span data-stu-id="ce2f9-133">id</span></span>|<span data-ttu-id="ce2f9-134">String</span><span class="sxs-lookup"><span data-stu-id="ce2f9-134">String</span></span>|<span data-ttu-id="ce2f9-135">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ce2f9-136">target</span><span class="sxs-lookup"><span data-stu-id="ce2f9-136">target</span></span>|[<span data-ttu-id="ce2f9-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ce2f9-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ce2f9-138">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="ce2f9-139">応答</span><span class="sxs-lookup"><span data-stu-id="ce2f9-139">Response</span></span>
<span data-ttu-id="ce2f9-140">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce2f9-141">例</span><span class="sxs-lookup"><span data-stu-id="ce2f9-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce2f9-142">要求</span><span class="sxs-lookup"><span data-stu-id="ce2f9-142">Request</span></span>
<span data-ttu-id="ce2f9-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ce2f9-144">応答</span><span class="sxs-lookup"><span data-stu-id="ce2f9-144">Response</span></span>
<span data-ttu-id="ce2f9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ce2f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




