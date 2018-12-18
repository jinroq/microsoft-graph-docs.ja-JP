---
title: managedEBookAssignment の作成
description: 新しい managedEBookAssignment オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 839052123c6ff0d4b4345ae8d8d0ad1bb921d674
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322954"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="9b4a7-103">managedEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="9b4a7-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="9b4a7-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b4a7-105">新しい [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-105">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b4a7-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="9b4a7-106">Prerequisites</span></span>
<span data-ttu-id="9b4a7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b4a7-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b4a7-109">Permission type</span></span>|<span data-ttu-id="9b4a7-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b4a7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b4a7-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b4a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9b4a7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b4a7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9b4a7-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b4a7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b4a7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-114">Not supported.</span></span>|
|<span data-ttu-id="9b4a7-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b4a7-115">Application</span></span>|<span data-ttu-id="9b4a7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b4a7-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b4a7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9b4a7-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b4a7-118">Request headers</span></span>
|<span data-ttu-id="9b4a7-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b4a7-119">Header</span></span>|<span data-ttu-id="9b4a7-120">値</span><span class="sxs-lookup"><span data-stu-id="9b4a7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b4a7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b4a7-121">Authorization</span></span>|<span data-ttu-id="9b4a7-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b4a7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9b4a7-123">Accept</span></span>|<span data-ttu-id="9b4a7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9b4a7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b4a7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9b4a7-125">Request body</span></span>
<span data-ttu-id="9b4a7-126">要求本文で、managedEBookAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-126">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="9b4a7-127">次の表に、managedEBookAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-127">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="9b4a7-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b4a7-128">Property</span></span>|<span data-ttu-id="9b4a7-129">種類</span><span class="sxs-lookup"><span data-stu-id="9b4a7-129">Type</span></span>|<span data-ttu-id="9b4a7-130">説明</span><span class="sxs-lookup"><span data-stu-id="9b4a7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b4a7-131">ID</span><span class="sxs-lookup"><span data-stu-id="9b4a7-131">id</span></span>|<span data-ttu-id="9b4a7-132">String</span><span class="sxs-lookup"><span data-stu-id="9b4a7-132">String</span></span>|<span data-ttu-id="9b4a7-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-133">Key of the entity.</span></span>|
|<span data-ttu-id="9b4a7-134">target</span><span class="sxs-lookup"><span data-stu-id="9b4a7-134">target</span></span>|[<span data-ttu-id="9b4a7-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9b4a7-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9b4a7-136">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="9b4a7-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="9b4a7-137">installIntent</span></span>|[<span data-ttu-id="9b4a7-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="9b4a7-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="9b4a7-139">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-139">The install intent for eBook.</span></span> <span data-ttu-id="9b4a7-140">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="9b4a7-141">応答</span><span class="sxs-lookup"><span data-stu-id="9b4a7-141">Response</span></span>
<span data-ttu-id="9b4a7-142">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-142">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b4a7-143">例</span><span class="sxs-lookup"><span data-stu-id="9b4a7-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b4a7-144">要求</span><span class="sxs-lookup"><span data-stu-id="9b4a7-144">Request</span></span>
<span data-ttu-id="9b4a7-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="9b4a7-146">応答</span><span class="sxs-lookup"><span data-stu-id="9b4a7-146">Response</span></span>
<span data-ttu-id="9b4a7-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9b4a7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



