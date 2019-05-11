---
title: managedEBookAssignment の更新
description: managedEBookAssignment オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f7bb4e95f4c32e0da8968833a2a69fbb5d8a26d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934188"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="97650-103">managedEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="97650-103">Update managedEBookAssignment</span></span>

> <span data-ttu-id="97650-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97650-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97650-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="97650-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97650-106">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="97650-106">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97650-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="97650-107">Prerequisites</span></span>
<span data-ttu-id="97650-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="97650-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97650-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="97650-110">Permission type</span></span>|<span data-ttu-id="97650-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="97650-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97650-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="97650-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97650-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97650-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="97650-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="97650-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97650-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97650-115">Not supported.</span></span>|
|<span data-ttu-id="97650-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="97650-116">Application</span></span>|<span data-ttu-id="97650-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97650-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97650-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="97650-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="97650-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="97650-119">Request headers</span></span>
|<span data-ttu-id="97650-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="97650-120">Header</span></span>|<span data-ttu-id="97650-121">値</span><span class="sxs-lookup"><span data-stu-id="97650-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97650-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="97650-122">Authorization</span></span>|<span data-ttu-id="97650-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="97650-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97650-124">承諾</span><span class="sxs-lookup"><span data-stu-id="97650-124">Accept</span></span>|<span data-ttu-id="97650-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97650-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97650-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="97650-126">Request body</span></span>
<span data-ttu-id="97650-127">要求本文で、[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="97650-127">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="97650-128">次の表に、[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="97650-128">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="97650-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97650-129">Property</span></span>|<span data-ttu-id="97650-130">型</span><span class="sxs-lookup"><span data-stu-id="97650-130">Type</span></span>|<span data-ttu-id="97650-131">説明</span><span class="sxs-lookup"><span data-stu-id="97650-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97650-132">id</span><span class="sxs-lookup"><span data-stu-id="97650-132">id</span></span>|<span data-ttu-id="97650-133">String</span><span class="sxs-lookup"><span data-stu-id="97650-133">String</span></span>|<span data-ttu-id="97650-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="97650-134">Key of the entity.</span></span>|
|<span data-ttu-id="97650-135">target</span><span class="sxs-lookup"><span data-stu-id="97650-135">target</span></span>|[<span data-ttu-id="97650-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="97650-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="97650-137">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="97650-137">The assignment target for eBook.</span></span>|
|<span data-ttu-id="97650-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="97650-138">installIntent</span></span>|[<span data-ttu-id="97650-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="97650-139">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="97650-140">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="97650-140">The install intent for eBook.</span></span> <span data-ttu-id="97650-141">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="97650-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="97650-142">応答</span><span class="sxs-lookup"><span data-stu-id="97650-142">Response</span></span>
<span data-ttu-id="97650-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="97650-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97650-144">例</span><span class="sxs-lookup"><span data-stu-id="97650-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="97650-145">要求</span><span class="sxs-lookup"><span data-stu-id="97650-145">Request</span></span>
<span data-ttu-id="97650-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="97650-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="97650-147">応答</span><span class="sxs-lookup"><span data-stu-id="97650-147">Response</span></span>
<span data-ttu-id="97650-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="97650-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




