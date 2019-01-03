---
title: iosVppEBookAssignment の更新
description: iosVppEBookAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 8a4970b41cae2ab164a1164970d15d0a8afec344
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330535"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="2659d-103">iosVppEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="2659d-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="2659d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2659d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2659d-105">[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2659d-105">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2659d-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="2659d-106">Prerequisites</span></span>
<span data-ttu-id="2659d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2659d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2659d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2659d-109">Permission type</span></span>|<span data-ttu-id="2659d-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2659d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2659d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2659d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2659d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2659d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2659d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2659d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2659d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2659d-114">Not supported.</span></span>|
|<span data-ttu-id="2659d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2659d-115">Application</span></span>|<span data-ttu-id="2659d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2659d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2659d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2659d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2659d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2659d-118">Request headers</span></span>
|<span data-ttu-id="2659d-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2659d-119">Header</span></span>|<span data-ttu-id="2659d-120">値</span><span class="sxs-lookup"><span data-stu-id="2659d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2659d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2659d-121">Authorization</span></span>|<span data-ttu-id="2659d-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2659d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2659d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2659d-123">Accept</span></span>|<span data-ttu-id="2659d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2659d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2659d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2659d-125">Request body</span></span>
<span data-ttu-id="2659d-126">要求本文で、[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2659d-126">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="2659d-127">次の表に、[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2659d-127">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="2659d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2659d-128">Property</span></span>|<span data-ttu-id="2659d-129">種類</span><span class="sxs-lookup"><span data-stu-id="2659d-129">Type</span></span>|<span data-ttu-id="2659d-130">説明</span><span class="sxs-lookup"><span data-stu-id="2659d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2659d-131">ID</span><span class="sxs-lookup"><span data-stu-id="2659d-131">id</span></span>|<span data-ttu-id="2659d-132">String</span><span class="sxs-lookup"><span data-stu-id="2659d-132">String</span></span>|<span data-ttu-id="2659d-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2659d-133">Key of the entity.</span></span> <span data-ttu-id="2659d-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2659d-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="2659d-135">target</span><span class="sxs-lookup"><span data-stu-id="2659d-135">target</span></span>|[<span data-ttu-id="2659d-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2659d-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2659d-137">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="2659d-137">The assignment target for eBook.</span></span> <span data-ttu-id="2659d-138">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2659d-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="2659d-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="2659d-139">installIntent</span></span>|[<span data-ttu-id="2659d-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="2659d-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="2659d-141">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="2659d-141">The install intent for eBook.</span></span> <span data-ttu-id="2659d-142">[ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="2659d-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="2659d-143">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="2659d-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="2659d-144">応答</span><span class="sxs-lookup"><span data-stu-id="2659d-144">Response</span></span>
<span data-ttu-id="2659d-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2659d-145">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2659d-146">例</span><span class="sxs-lookup"><span data-stu-id="2659d-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="2659d-147">要求</span><span class="sxs-lookup"><span data-stu-id="2659d-147">Request</span></span>
<span data-ttu-id="2659d-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2659d-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2659d-149">応答</span><span class="sxs-lookup"><span data-stu-id="2659d-149">Response</span></span>
<span data-ttu-id="2659d-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2659d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


