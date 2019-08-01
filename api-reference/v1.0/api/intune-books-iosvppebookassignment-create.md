---
title: iosVppEBookAssignment の作成
description: 新しい iosVppEBookAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56a560c45be3c1932636c988c11359125469b6b3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013585"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="9a6c6-103">iosVppEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="9a6c6-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="9a6c6-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a6c6-105">新しい [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-105">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a6c6-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="9a6c6-106">Prerequisites</span></span>
<span data-ttu-id="9a6c6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a6c6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a6c6-109">Permission type</span></span>|<span data-ttu-id="9a6c6-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a6c6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a6c6-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a6c6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9a6c6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a6c6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9a6c6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a6c6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a6c6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-114">Not supported.</span></span>|
|<span data-ttu-id="9a6c6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a6c6-115">Application</span></span>|<span data-ttu-id="9a6c6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a6c6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a6c6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9a6c6-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a6c6-118">Request headers</span></span>
|<span data-ttu-id="9a6c6-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a6c6-119">Header</span></span>|<span data-ttu-id="9a6c6-120">値</span><span class="sxs-lookup"><span data-stu-id="9a6c6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a6c6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a6c6-121">Authorization</span></span>|<span data-ttu-id="9a6c6-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a6c6-123">承諾</span><span class="sxs-lookup"><span data-stu-id="9a6c6-123">Accept</span></span>|<span data-ttu-id="9a6c6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9a6c6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a6c6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a6c6-125">Request body</span></span>
<span data-ttu-id="9a6c6-126">要求本文で、iosVppEBookAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-126">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="9a6c6-127">次の表に、iosVppEBookAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-127">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="9a6c6-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a6c6-128">Property</span></span>|<span data-ttu-id="9a6c6-129">型</span><span class="sxs-lookup"><span data-stu-id="9a6c6-129">Type</span></span>|<span data-ttu-id="9a6c6-130">説明</span><span class="sxs-lookup"><span data-stu-id="9a6c6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a6c6-131">id</span><span class="sxs-lookup"><span data-stu-id="9a6c6-131">id</span></span>|<span data-ttu-id="9a6c6-132">String</span><span class="sxs-lookup"><span data-stu-id="9a6c6-132">String</span></span>|<span data-ttu-id="9a6c6-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-133">Key of the entity.</span></span> <span data-ttu-id="9a6c6-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a6c6-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="9a6c6-135">target</span><span class="sxs-lookup"><span data-stu-id="9a6c6-135">target</span></span>|[<span data-ttu-id="9a6c6-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9a6c6-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9a6c6-137">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-137">The assignment target for eBook.</span></span> <span data-ttu-id="9a6c6-138">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a6c6-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="9a6c6-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="9a6c6-139">installIntent</span></span>|[<span data-ttu-id="9a6c6-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="9a6c6-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="9a6c6-141">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-141">The install intent for eBook.</span></span> <span data-ttu-id="9a6c6-142">[Managedebookassignment](../resources/intune-books-managedebookassignment.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="9a6c6-143">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="9a6c6-144">応答</span><span class="sxs-lookup"><span data-stu-id="9a6c6-144">Response</span></span>
<span data-ttu-id="9a6c6-145">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-145">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a6c6-146">例</span><span class="sxs-lookup"><span data-stu-id="9a6c6-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a6c6-147">要求</span><span class="sxs-lookup"><span data-stu-id="9a6c6-147">Request</span></span>
<span data-ttu-id="9a6c6-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="9a6c6-149">応答</span><span class="sxs-lookup"><span data-stu-id="9a6c6-149">Response</span></span>
<span data-ttu-id="9a6c6-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9a6c6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



