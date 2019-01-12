---
title: iosVppEBookAssignment の作成
description: 新しい iosVppEBookAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b5ff460b702c943268d9992bd17e99fd54369548
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963970"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="6cff9-103">iosVppEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="6cff9-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="6cff9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6cff9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cff9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cff9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6cff9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6cff9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cff9-107">新しい [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6cff9-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6cff9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="6cff9-108">Prerequisites</span></span>
<span data-ttu-id="6cff9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6cff9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cff9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6cff9-111">Permission type</span></span>|<span data-ttu-id="6cff9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6cff9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cff9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6cff9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cff9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cff9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6cff9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6cff9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cff9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cff9-116">Not supported.</span></span>|
|<span data-ttu-id="6cff9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6cff9-117">Application</span></span>|<span data-ttu-id="6cff9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cff9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cff9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6cff9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6cff9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6cff9-120">Request headers</span></span>
|<span data-ttu-id="6cff9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6cff9-121">Header</span></span>|<span data-ttu-id="6cff9-122">値</span><span class="sxs-lookup"><span data-stu-id="6cff9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cff9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cff9-123">Authorization</span></span>|<span data-ttu-id="6cff9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6cff9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cff9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6cff9-125">Accept</span></span>|<span data-ttu-id="6cff9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cff9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cff9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6cff9-127">Request body</span></span>
<span data-ttu-id="6cff9-128">要求本文で、iosVppEBookAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6cff9-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="6cff9-129">次の表に、iosVppEBookAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6cff9-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="6cff9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6cff9-130">Property</span></span>|<span data-ttu-id="6cff9-131">種類</span><span class="sxs-lookup"><span data-stu-id="6cff9-131">Type</span></span>|<span data-ttu-id="6cff9-132">説明</span><span class="sxs-lookup"><span data-stu-id="6cff9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cff9-133">ID</span><span class="sxs-lookup"><span data-stu-id="6cff9-133">id</span></span>|<span data-ttu-id="6cff9-134">String</span><span class="sxs-lookup"><span data-stu-id="6cff9-134">String</span></span>|<span data-ttu-id="6cff9-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6cff9-135">Key of the entity.</span></span> <span data-ttu-id="6cff9-136">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cff9-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="6cff9-137">target</span><span class="sxs-lookup"><span data-stu-id="6cff9-137">target</span></span>|[<span data-ttu-id="6cff9-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6cff9-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6cff9-139">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="6cff9-139">The assignment target for eBook.</span></span> <span data-ttu-id="6cff9-140">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cff9-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="6cff9-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="6cff9-141">installIntent</span></span>|[<span data-ttu-id="6cff9-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="6cff9-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="6cff9-143">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="6cff9-143">The install intent for eBook.</span></span> <span data-ttu-id="6cff9-144">[ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="6cff9-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="6cff9-145">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="6cff9-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="6cff9-146">応答</span><span class="sxs-lookup"><span data-stu-id="6cff9-146">Response</span></span>
<span data-ttu-id="6cff9-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6cff9-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cff9-148">例</span><span class="sxs-lookup"><span data-stu-id="6cff9-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="6cff9-149">要求</span><span class="sxs-lookup"><span data-stu-id="6cff9-149">Request</span></span>
<span data-ttu-id="6cff9-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6cff9-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="6cff9-151">応答</span><span class="sxs-lookup"><span data-stu-id="6cff9-151">Response</span></span>
<span data-ttu-id="6cff9-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6cff9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





