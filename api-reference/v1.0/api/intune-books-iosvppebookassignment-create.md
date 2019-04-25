---
title: iosVppEBookAssignment の作成
description: 新しい iosVppEBookAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b45e4a986306fbecf039abee29c2a6939f9b4e69
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577127"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="6933e-103">iosVppEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="6933e-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="6933e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6933e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6933e-105">新しい [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6933e-105">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6933e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6933e-106">Prerequisites</span></span>
<span data-ttu-id="6933e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6933e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6933e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6933e-109">Permission type</span></span>|<span data-ttu-id="6933e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6933e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6933e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6933e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6933e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6933e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6933e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6933e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6933e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6933e-114">Not supported.</span></span>|
|<span data-ttu-id="6933e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6933e-115">Application</span></span>|<span data-ttu-id="6933e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6933e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6933e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6933e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6933e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6933e-118">Request headers</span></span>
|<span data-ttu-id="6933e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6933e-119">Header</span></span>|<span data-ttu-id="6933e-120">値</span><span class="sxs-lookup"><span data-stu-id="6933e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6933e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6933e-121">Authorization</span></span>|<span data-ttu-id="6933e-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6933e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6933e-123">承諾</span><span class="sxs-lookup"><span data-stu-id="6933e-123">Accept</span></span>|<span data-ttu-id="6933e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6933e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6933e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6933e-125">Request body</span></span>
<span data-ttu-id="6933e-126">要求本文で、iosVppEBookAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6933e-126">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="6933e-127">次の表に、iosVppEBookAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6933e-127">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="6933e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6933e-128">Property</span></span>|<span data-ttu-id="6933e-129">型</span><span class="sxs-lookup"><span data-stu-id="6933e-129">Type</span></span>|<span data-ttu-id="6933e-130">説明</span><span class="sxs-lookup"><span data-stu-id="6933e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6933e-131">id</span><span class="sxs-lookup"><span data-stu-id="6933e-131">id</span></span>|<span data-ttu-id="6933e-132">String</span><span class="sxs-lookup"><span data-stu-id="6933e-132">String</span></span>|<span data-ttu-id="6933e-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6933e-133">Key of the entity.</span></span> <span data-ttu-id="6933e-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6933e-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="6933e-135">target</span><span class="sxs-lookup"><span data-stu-id="6933e-135">target</span></span>|[<span data-ttu-id="6933e-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6933e-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6933e-137">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="6933e-137">The assignment target for eBook.</span></span> <span data-ttu-id="6933e-138">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6933e-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="6933e-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="6933e-139">installIntent</span></span>|[<span data-ttu-id="6933e-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="6933e-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="6933e-141">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="6933e-141">The install intent for eBook.</span></span> <span data-ttu-id="6933e-142">[managedebookassignment](../resources/intune-books-managedebookassignment.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6933e-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="6933e-143">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="6933e-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="6933e-144">応答</span><span class="sxs-lookup"><span data-stu-id="6933e-144">Response</span></span>
<span data-ttu-id="6933e-145">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6933e-145">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6933e-146">例</span><span class="sxs-lookup"><span data-stu-id="6933e-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="6933e-147">要求</span><span class="sxs-lookup"><span data-stu-id="6933e-147">Request</span></span>
<span data-ttu-id="6933e-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6933e-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6933e-149">応答</span><span class="sxs-lookup"><span data-stu-id="6933e-149">Response</span></span>
<span data-ttu-id="6933e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6933e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



