---
title: iosVppEBookAssignment の更新
description: iosVppEBookAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1af37aaf787c7909d1d3653d196ebb19b68476cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524964"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="e65db-103">iosVppEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="e65db-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="e65db-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e65db-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e65db-105">[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e65db-105">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e65db-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="e65db-106">Prerequisites</span></span>
<span data-ttu-id="e65db-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e65db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e65db-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e65db-109">Permission type</span></span>|<span data-ttu-id="e65db-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e65db-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e65db-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e65db-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e65db-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e65db-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e65db-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e65db-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e65db-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e65db-114">Not supported.</span></span>|
|<span data-ttu-id="e65db-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e65db-115">Application</span></span>|<span data-ttu-id="e65db-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e65db-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e65db-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e65db-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e65db-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e65db-118">Request headers</span></span>
|<span data-ttu-id="e65db-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e65db-119">Header</span></span>|<span data-ttu-id="e65db-120">値</span><span class="sxs-lookup"><span data-stu-id="e65db-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e65db-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e65db-121">Authorization</span></span>|<span data-ttu-id="e65db-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e65db-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e65db-123">承諾</span><span class="sxs-lookup"><span data-stu-id="e65db-123">Accept</span></span>|<span data-ttu-id="e65db-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e65db-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e65db-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e65db-125">Request body</span></span>
<span data-ttu-id="e65db-126">要求本文で、[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e65db-126">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="e65db-127">次の表に、[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e65db-127">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="e65db-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e65db-128">Property</span></span>|<span data-ttu-id="e65db-129">型</span><span class="sxs-lookup"><span data-stu-id="e65db-129">Type</span></span>|<span data-ttu-id="e65db-130">説明</span><span class="sxs-lookup"><span data-stu-id="e65db-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e65db-131">id</span><span class="sxs-lookup"><span data-stu-id="e65db-131">id</span></span>|<span data-ttu-id="e65db-132">String</span><span class="sxs-lookup"><span data-stu-id="e65db-132">String</span></span>|<span data-ttu-id="e65db-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e65db-133">Key of the entity.</span></span> <span data-ttu-id="e65db-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e65db-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="e65db-135">target</span><span class="sxs-lookup"><span data-stu-id="e65db-135">target</span></span>|[<span data-ttu-id="e65db-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e65db-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e65db-137">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="e65db-137">The assignment target for eBook.</span></span> <span data-ttu-id="e65db-138">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e65db-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="e65db-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="e65db-139">installIntent</span></span>|[<span data-ttu-id="e65db-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="e65db-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="e65db-141">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="e65db-141">The install intent for eBook.</span></span> <span data-ttu-id="e65db-142">[managedebookassignment](../resources/intune-books-managedebookassignment.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e65db-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="e65db-143">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="e65db-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="e65db-144">応答</span><span class="sxs-lookup"><span data-stu-id="e65db-144">Response</span></span>
<span data-ttu-id="e65db-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e65db-145">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e65db-146">例</span><span class="sxs-lookup"><span data-stu-id="e65db-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="e65db-147">要求</span><span class="sxs-lookup"><span data-stu-id="e65db-147">Request</span></span>
<span data-ttu-id="e65db-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e65db-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e65db-149">応答</span><span class="sxs-lookup"><span data-stu-id="e65db-149">Response</span></span>
<span data-ttu-id="e65db-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e65db-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



