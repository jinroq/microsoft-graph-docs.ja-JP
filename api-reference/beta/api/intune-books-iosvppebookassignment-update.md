---
title: iosVppEBookAssignment の更新
description: iosVppEBookAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c04bd5a2a6e57d64a1baed1a80cb6e6c2761a00
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158479"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="2d8d5-103">iosVppEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="2d8d5-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="2d8d5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d8d5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d8d5-106">[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-106">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d8d5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2d8d5-107">Prerequisites</span></span>
<span data-ttu-id="2d8d5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2d8d5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2d8d5-110">Permission type</span></span>|<span data-ttu-id="2d8d5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2d8d5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d8d5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2d8d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d8d5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d8d5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2d8d5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2d8d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d8d5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-115">Not supported.</span></span>|
|<span data-ttu-id="2d8d5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2d8d5-116">Application</span></span>|<span data-ttu-id="2d8d5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d8d5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2d8d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2d8d5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d8d5-119">Request headers</span></span>
|<span data-ttu-id="2d8d5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d8d5-120">Header</span></span>|<span data-ttu-id="2d8d5-121">値</span><span class="sxs-lookup"><span data-stu-id="2d8d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d8d5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d8d5-122">Authorization</span></span>|<span data-ttu-id="2d8d5-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d8d5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2d8d5-124">Accept</span></span>|<span data-ttu-id="2d8d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d8d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d8d5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2d8d5-126">Request body</span></span>
<span data-ttu-id="2d8d5-127">要求本文で、[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-127">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="2d8d5-128">次の表に、[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-128">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="2d8d5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d8d5-129">Property</span></span>|<span data-ttu-id="2d8d5-130">型</span><span class="sxs-lookup"><span data-stu-id="2d8d5-130">Type</span></span>|<span data-ttu-id="2d8d5-131">説明</span><span class="sxs-lookup"><span data-stu-id="2d8d5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d8d5-132">id</span><span class="sxs-lookup"><span data-stu-id="2d8d5-132">id</span></span>|<span data-ttu-id="2d8d5-133">String</span><span class="sxs-lookup"><span data-stu-id="2d8d5-133">String</span></span>|<span data-ttu-id="2d8d5-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-134">Key of the entity.</span></span> <span data-ttu-id="2d8d5-135">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d8d5-135">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="2d8d5-136">target</span><span class="sxs-lookup"><span data-stu-id="2d8d5-136">target</span></span>|[<span data-ttu-id="2d8d5-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2d8d5-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2d8d5-138">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-138">The assignment target for eBook.</span></span> <span data-ttu-id="2d8d5-139">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d8d5-139">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="2d8d5-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="2d8d5-140">installIntent</span></span>|[<span data-ttu-id="2d8d5-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="2d8d5-141">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="2d8d5-142">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-142">The install intent for eBook.</span></span> <span data-ttu-id="2d8d5-143">[managedebookassignment](../resources/intune-books-managedebookassignment.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-143">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="2d8d5-144">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-144">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="2d8d5-145">応答</span><span class="sxs-lookup"><span data-stu-id="2d8d5-145">Response</span></span>
<span data-ttu-id="2d8d5-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-146">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d8d5-147">例</span><span class="sxs-lookup"><span data-stu-id="2d8d5-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d8d5-148">要求</span><span class="sxs-lookup"><span data-stu-id="2d8d5-148">Request</span></span>
<span data-ttu-id="2d8d5-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="2d8d5-150">応答</span><span class="sxs-lookup"><span data-stu-id="2d8d5-150">Response</span></span>
<span data-ttu-id="2d8d5-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2d8d5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




