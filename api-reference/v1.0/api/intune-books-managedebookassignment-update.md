---
title: managedEBookAssignment の更新
description: managedEBookAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cad8ce31a9de355b79407ee4658ea13ef0415732
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804964"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="26c35-103">managedEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="26c35-103">Update managedEBookAssignment</span></span>

> <span data-ttu-id="26c35-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="26c35-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26c35-105">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="26c35-105">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="26c35-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="26c35-106">Prerequisites</span></span>
<span data-ttu-id="26c35-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26c35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26c35-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26c35-109">Permission type</span></span>|<span data-ttu-id="26c35-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="26c35-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26c35-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26c35-111">Delegated (work or school account)</span></span>|<span data-ttu-id="26c35-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26c35-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="26c35-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26c35-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26c35-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26c35-114">Not supported.</span></span>|
|<span data-ttu-id="26c35-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26c35-115">Application</span></span>|<span data-ttu-id="26c35-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26c35-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26c35-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26c35-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="26c35-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26c35-118">Request headers</span></span>
|<span data-ttu-id="26c35-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26c35-119">Header</span></span>|<span data-ttu-id="26c35-120">値</span><span class="sxs-lookup"><span data-stu-id="26c35-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26c35-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="26c35-121">Authorization</span></span>|<span data-ttu-id="26c35-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="26c35-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26c35-123">Accept</span><span class="sxs-lookup"><span data-stu-id="26c35-123">Accept</span></span>|<span data-ttu-id="26c35-124">application/json</span><span class="sxs-lookup"><span data-stu-id="26c35-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26c35-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="26c35-125">Request body</span></span>
<span data-ttu-id="26c35-126">要求本文で、[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="26c35-126">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="26c35-127">次の表に、[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="26c35-127">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="26c35-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26c35-128">Property</span></span>|<span data-ttu-id="26c35-129">種類</span><span class="sxs-lookup"><span data-stu-id="26c35-129">Type</span></span>|<span data-ttu-id="26c35-130">説明</span><span class="sxs-lookup"><span data-stu-id="26c35-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26c35-131">ID</span><span class="sxs-lookup"><span data-stu-id="26c35-131">id</span></span>|<span data-ttu-id="26c35-132">String</span><span class="sxs-lookup"><span data-stu-id="26c35-132">String</span></span>|<span data-ttu-id="26c35-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="26c35-133">Key of the entity.</span></span>|
|<span data-ttu-id="26c35-134">target</span><span class="sxs-lookup"><span data-stu-id="26c35-134">target</span></span>|[<span data-ttu-id="26c35-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="26c35-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="26c35-136">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="26c35-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="26c35-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="26c35-137">installIntent</span></span>|[<span data-ttu-id="26c35-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="26c35-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="26c35-139">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="26c35-139">The install intent for eBook.</span></span> <span data-ttu-id="26c35-140">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="26c35-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="26c35-141">応答</span><span class="sxs-lookup"><span data-stu-id="26c35-141">Response</span></span>
<span data-ttu-id="26c35-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="26c35-142">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26c35-143">例</span><span class="sxs-lookup"><span data-stu-id="26c35-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="26c35-144">要求</span><span class="sxs-lookup"><span data-stu-id="26c35-144">Request</span></span>
<span data-ttu-id="26c35-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="26c35-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="26c35-146">応答</span><span class="sxs-lookup"><span data-stu-id="26c35-146">Response</span></span>
<span data-ttu-id="26c35-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="26c35-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



