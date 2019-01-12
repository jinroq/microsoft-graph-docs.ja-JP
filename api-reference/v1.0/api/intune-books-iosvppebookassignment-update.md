---
title: iosVppEBookAssignment の更新
description: iosVppEBookAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4521068ab7b278b8d7f4c0d485c3d97f1c1d8b0a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912415"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="a408f-103">iosVppEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="a408f-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="a408f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a408f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a408f-105">[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a408f-105">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a408f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a408f-106">Prerequisites</span></span>
<span data-ttu-id="a408f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a408f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a408f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a408f-109">Permission type</span></span>|<span data-ttu-id="a408f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a408f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a408f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a408f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a408f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a408f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a408f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a408f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a408f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a408f-114">Not supported.</span></span>|
|<span data-ttu-id="a408f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a408f-115">Application</span></span>|<span data-ttu-id="a408f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a408f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a408f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a408f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="a408f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a408f-118">Request headers</span></span>
|<span data-ttu-id="a408f-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a408f-119">Header</span></span>|<span data-ttu-id="a408f-120">値</span><span class="sxs-lookup"><span data-stu-id="a408f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a408f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a408f-121">Authorization</span></span>|<span data-ttu-id="a408f-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a408f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a408f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a408f-123">Accept</span></span>|<span data-ttu-id="a408f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a408f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a408f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a408f-125">Request body</span></span>
<span data-ttu-id="a408f-126">要求本文で、[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a408f-126">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="a408f-127">次の表に、[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a408f-127">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="a408f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a408f-128">Property</span></span>|<span data-ttu-id="a408f-129">型</span><span class="sxs-lookup"><span data-stu-id="a408f-129">Type</span></span>|<span data-ttu-id="a408f-130">説明</span><span class="sxs-lookup"><span data-stu-id="a408f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a408f-131">ID</span><span class="sxs-lookup"><span data-stu-id="a408f-131">id</span></span>|<span data-ttu-id="a408f-132">String</span><span class="sxs-lookup"><span data-stu-id="a408f-132">String</span></span>|<span data-ttu-id="a408f-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a408f-133">Key of the entity.</span></span> <span data-ttu-id="a408f-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a408f-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="a408f-135">target</span><span class="sxs-lookup"><span data-stu-id="a408f-135">target</span></span>|[<span data-ttu-id="a408f-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a408f-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a408f-137">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="a408f-137">The assignment target for eBook.</span></span> <span data-ttu-id="a408f-138">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a408f-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="a408f-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="a408f-139">installIntent</span></span>|[<span data-ttu-id="a408f-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="a408f-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="a408f-141">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="a408f-141">The install intent for eBook.</span></span> <span data-ttu-id="a408f-142">[ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a408f-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="a408f-143">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="a408f-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="a408f-144">応答</span><span class="sxs-lookup"><span data-stu-id="a408f-144">Response</span></span>
<span data-ttu-id="a408f-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a408f-145">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a408f-146">例</span><span class="sxs-lookup"><span data-stu-id="a408f-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="a408f-147">要求</span><span class="sxs-lookup"><span data-stu-id="a408f-147">Request</span></span>
<span data-ttu-id="a408f-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a408f-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="a408f-149">応答</span><span class="sxs-lookup"><span data-stu-id="a408f-149">Response</span></span>
<span data-ttu-id="a408f-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a408f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "48f05789-5789-48f0-8957-f0488957f048",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



