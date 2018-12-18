---
title: iosVppEBookAssignment の更新
description: iosVppEBookAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 537c2ef5838dc68881f3de693a6591570219ece4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338151"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="0cafb-103">iosVppEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="0cafb-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="0cafb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0cafb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0cafb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cafb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0cafb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0cafb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0cafb-107">[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0cafb-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0cafb-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0cafb-108">Prerequisites</span></span>
<span data-ttu-id="0cafb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0cafb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cafb-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0cafb-111">Permission type</span></span>|<span data-ttu-id="0cafb-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0cafb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cafb-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0cafb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0cafb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cafb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0cafb-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0cafb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cafb-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cafb-116">Not supported.</span></span>|
|<span data-ttu-id="0cafb-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0cafb-117">Application</span></span>|<span data-ttu-id="0cafb-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cafb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cafb-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0cafb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="0cafb-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cafb-120">Request headers</span></span>
|<span data-ttu-id="0cafb-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cafb-121">Header</span></span>|<span data-ttu-id="0cafb-122">値</span><span class="sxs-lookup"><span data-stu-id="0cafb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cafb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cafb-123">Authorization</span></span>|<span data-ttu-id="0cafb-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0cafb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cafb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0cafb-125">Accept</span></span>|<span data-ttu-id="0cafb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0cafb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cafb-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0cafb-127">Request body</span></span>
<span data-ttu-id="0cafb-128">要求本文で、[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0cafb-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="0cafb-129">次の表に、[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0cafb-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="0cafb-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cafb-130">Property</span></span>|<span data-ttu-id="0cafb-131">種類</span><span class="sxs-lookup"><span data-stu-id="0cafb-131">Type</span></span>|<span data-ttu-id="0cafb-132">説明</span><span class="sxs-lookup"><span data-stu-id="0cafb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cafb-133">ID</span><span class="sxs-lookup"><span data-stu-id="0cafb-133">id</span></span>|<span data-ttu-id="0cafb-134">String</span><span class="sxs-lookup"><span data-stu-id="0cafb-134">String</span></span>|<span data-ttu-id="0cafb-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0cafb-135">Key of the entity.</span></span> <span data-ttu-id="0cafb-136">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0cafb-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="0cafb-137">target</span><span class="sxs-lookup"><span data-stu-id="0cafb-137">target</span></span>|[<span data-ttu-id="0cafb-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0cafb-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0cafb-139">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="0cafb-139">The assignment target for eBook.</span></span> <span data-ttu-id="0cafb-140">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0cafb-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="0cafb-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="0cafb-141">installIntent</span></span>|[<span data-ttu-id="0cafb-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="0cafb-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="0cafb-143">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="0cafb-143">The install intent for eBook.</span></span> <span data-ttu-id="0cafb-144">[ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="0cafb-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="0cafb-145">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="0cafb-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="0cafb-146">応答</span><span class="sxs-lookup"><span data-stu-id="0cafb-146">Response</span></span>
<span data-ttu-id="0cafb-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0cafb-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cafb-148">例</span><span class="sxs-lookup"><span data-stu-id="0cafb-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="0cafb-149">要求</span><span class="sxs-lookup"><span data-stu-id="0cafb-149">Request</span></span>
<span data-ttu-id="0cafb-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0cafb-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 133

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="0cafb-151">応答</span><span class="sxs-lookup"><span data-stu-id="0cafb-151">Response</span></span>
<span data-ttu-id="0cafb-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0cafb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





