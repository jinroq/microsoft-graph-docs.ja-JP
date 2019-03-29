---
title: managedEBookAssignment の更新
description: managedEBookAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12f703c7d1cd467aff6bfff9bf14c4954870bff7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982659"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="67897-103">managedEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="67897-103">Update managedEBookAssignment</span></span>

> <span data-ttu-id="67897-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="67897-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67897-105">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="67897-105">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67897-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="67897-106">Prerequisites</span></span>
<span data-ttu-id="67897-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67897-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67897-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67897-109">Permission type</span></span>|<span data-ttu-id="67897-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="67897-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67897-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67897-111">Delegated (work or school account)</span></span>|<span data-ttu-id="67897-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67897-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="67897-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67897-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67897-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67897-114">Not supported.</span></span>|
|<span data-ttu-id="67897-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67897-115">Application</span></span>|<span data-ttu-id="67897-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67897-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67897-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67897-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="67897-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67897-118">Request headers</span></span>
|<span data-ttu-id="67897-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67897-119">Header</span></span>|<span data-ttu-id="67897-120">値</span><span class="sxs-lookup"><span data-stu-id="67897-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67897-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67897-121">Authorization</span></span>|<span data-ttu-id="67897-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="67897-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67897-123">承諾</span><span class="sxs-lookup"><span data-stu-id="67897-123">Accept</span></span>|<span data-ttu-id="67897-124">application/json</span><span class="sxs-lookup"><span data-stu-id="67897-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67897-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="67897-125">Request body</span></span>
<span data-ttu-id="67897-126">要求本文で、[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="67897-126">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="67897-127">次の表に、[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="67897-127">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="67897-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67897-128">Property</span></span>|<span data-ttu-id="67897-129">型</span><span class="sxs-lookup"><span data-stu-id="67897-129">Type</span></span>|<span data-ttu-id="67897-130">説明</span><span class="sxs-lookup"><span data-stu-id="67897-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67897-131">id</span><span class="sxs-lookup"><span data-stu-id="67897-131">id</span></span>|<span data-ttu-id="67897-132">String</span><span class="sxs-lookup"><span data-stu-id="67897-132">String</span></span>|<span data-ttu-id="67897-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="67897-133">Key of the entity.</span></span>|
|<span data-ttu-id="67897-134">target</span><span class="sxs-lookup"><span data-stu-id="67897-134">target</span></span>|[<span data-ttu-id="67897-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="67897-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="67897-136">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="67897-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="67897-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="67897-137">installIntent</span></span>|[<span data-ttu-id="67897-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="67897-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="67897-139">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="67897-139">The install intent for eBook.</span></span> <span data-ttu-id="67897-140">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="67897-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="67897-141">応答</span><span class="sxs-lookup"><span data-stu-id="67897-141">Response</span></span>
<span data-ttu-id="67897-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="67897-142">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67897-143">例</span><span class="sxs-lookup"><span data-stu-id="67897-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="67897-144">要求</span><span class="sxs-lookup"><span data-stu-id="67897-144">Request</span></span>
<span data-ttu-id="67897-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67897-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="67897-146">応答</span><span class="sxs-lookup"><span data-stu-id="67897-146">Response</span></span>
<span data-ttu-id="67897-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67897-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



