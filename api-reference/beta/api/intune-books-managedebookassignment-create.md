---
title: managedEBookAssignment の作成
description: 新しい managedEBookAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ad6d30b07bd128572500be7a1a85fa4ae1333e6c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935207"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="b851d-103">managedEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="b851d-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="b851d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b851d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b851d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b851d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b851d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b851d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b851d-107">新しい [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b851d-107">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b851d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b851d-108">Prerequisites</span></span>
<span data-ttu-id="b851d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b851d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b851d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b851d-111">Permission type</span></span>|<span data-ttu-id="b851d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b851d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b851d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b851d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b851d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b851d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b851d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b851d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b851d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b851d-116">Not supported.</span></span>|
|<span data-ttu-id="b851d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b851d-117">Application</span></span>|<span data-ttu-id="b851d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b851d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b851d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b851d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b851d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b851d-120">Request headers</span></span>
|<span data-ttu-id="b851d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b851d-121">Header</span></span>|<span data-ttu-id="b851d-122">値</span><span class="sxs-lookup"><span data-stu-id="b851d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b851d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b851d-123">Authorization</span></span>|<span data-ttu-id="b851d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b851d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b851d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b851d-125">Accept</span></span>|<span data-ttu-id="b851d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b851d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b851d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b851d-127">Request body</span></span>
<span data-ttu-id="b851d-128">要求本文で、managedEBookAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b851d-128">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="b851d-129">次の表に、managedEBookAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b851d-129">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="b851d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b851d-130">Property</span></span>|<span data-ttu-id="b851d-131">型</span><span class="sxs-lookup"><span data-stu-id="b851d-131">Type</span></span>|<span data-ttu-id="b851d-132">説明</span><span class="sxs-lookup"><span data-stu-id="b851d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b851d-133">ID</span><span class="sxs-lookup"><span data-stu-id="b851d-133">id</span></span>|<span data-ttu-id="b851d-134">String</span><span class="sxs-lookup"><span data-stu-id="b851d-134">String</span></span>|<span data-ttu-id="b851d-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b851d-135">Key of the entity.</span></span>|
|<span data-ttu-id="b851d-136">target</span><span class="sxs-lookup"><span data-stu-id="b851d-136">target</span></span>|[<span data-ttu-id="b851d-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b851d-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b851d-138">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="b851d-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="b851d-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="b851d-139">installIntent</span></span>|[<span data-ttu-id="b851d-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="b851d-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="b851d-141">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="b851d-141">The install intent for eBook.</span></span> <span data-ttu-id="b851d-142">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="b851d-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="b851d-143">応答</span><span class="sxs-lookup"><span data-stu-id="b851d-143">Response</span></span>
<span data-ttu-id="b851d-144">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b851d-144">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b851d-145">例</span><span class="sxs-lookup"><span data-stu-id="b851d-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="b851d-146">要求</span><span class="sxs-lookup"><span data-stu-id="b851d-146">Request</span></span>
<span data-ttu-id="b851d-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b851d-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b851d-148">応答</span><span class="sxs-lookup"><span data-stu-id="b851d-148">Response</span></span>
<span data-ttu-id="b851d-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b851d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





