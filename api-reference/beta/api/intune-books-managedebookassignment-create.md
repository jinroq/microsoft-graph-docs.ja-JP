---
title: managedEBookAssignment の作成
description: 新しい managedEBookAssignment オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ebb4f0bede59a636085c813fa49533015802b6a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959195"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="7152c-103">managedEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="7152c-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="7152c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7152c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7152c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7152c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7152c-106">新しい [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7152c-106">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7152c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7152c-107">Prerequisites</span></span>
<span data-ttu-id="7152c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7152c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7152c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7152c-110">Permission type</span></span>|<span data-ttu-id="7152c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7152c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7152c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7152c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7152c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7152c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7152c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7152c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7152c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7152c-115">Not supported.</span></span>|
|<span data-ttu-id="7152c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7152c-116">Application</span></span>|<span data-ttu-id="7152c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7152c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7152c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7152c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7152c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7152c-119">Request headers</span></span>
|<span data-ttu-id="7152c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7152c-120">Header</span></span>|<span data-ttu-id="7152c-121">値</span><span class="sxs-lookup"><span data-stu-id="7152c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7152c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7152c-122">Authorization</span></span>|<span data-ttu-id="7152c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7152c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7152c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7152c-124">Accept</span></span>|<span data-ttu-id="7152c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7152c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7152c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7152c-126">Request body</span></span>
<span data-ttu-id="7152c-127">要求本文で、managedEBookAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7152c-127">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="7152c-128">次の表に、managedEBookAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7152c-128">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="7152c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7152c-129">Property</span></span>|<span data-ttu-id="7152c-130">型</span><span class="sxs-lookup"><span data-stu-id="7152c-130">Type</span></span>|<span data-ttu-id="7152c-131">説明</span><span class="sxs-lookup"><span data-stu-id="7152c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7152c-132">id</span><span class="sxs-lookup"><span data-stu-id="7152c-132">id</span></span>|<span data-ttu-id="7152c-133">String</span><span class="sxs-lookup"><span data-stu-id="7152c-133">String</span></span>|<span data-ttu-id="7152c-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7152c-134">Key of the entity.</span></span>|
|<span data-ttu-id="7152c-135">target</span><span class="sxs-lookup"><span data-stu-id="7152c-135">target</span></span>|[<span data-ttu-id="7152c-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7152c-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7152c-137">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="7152c-137">The assignment target for eBook.</span></span>|
|<span data-ttu-id="7152c-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="7152c-138">installIntent</span></span>|[<span data-ttu-id="7152c-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="7152c-139">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="7152c-140">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="7152c-140">The install intent for eBook.</span></span> <span data-ttu-id="7152c-141">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="7152c-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="7152c-142">応答</span><span class="sxs-lookup"><span data-stu-id="7152c-142">Response</span></span>
<span data-ttu-id="7152c-143">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7152c-143">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7152c-144">例</span><span class="sxs-lookup"><span data-stu-id="7152c-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="7152c-145">要求</span><span class="sxs-lookup"><span data-stu-id="7152c-145">Request</span></span>
<span data-ttu-id="7152c-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7152c-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="7152c-147">応答</span><span class="sxs-lookup"><span data-stu-id="7152c-147">Response</span></span>
<span data-ttu-id="7152c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7152c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





