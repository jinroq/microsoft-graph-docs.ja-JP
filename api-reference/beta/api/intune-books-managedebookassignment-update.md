---
title: managedEBookAssignment の更新
description: managedEBookAssignment オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0cf6aef49315eba7f6c67af34147a577a43a5a80
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413795"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="3bb2f-103">managedEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="3bb2f-103">Update managedEBookAssignment</span></span>

> <span data-ttu-id="3bb2f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3bb2f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3bb2f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bb2f-107">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-107">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bb2f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3bb2f-108">Prerequisites</span></span>
<span data-ttu-id="3bb2f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3bb2f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3bb2f-111">Permission type</span></span>|<span data-ttu-id="3bb2f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3bb2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bb2f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3bb2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3bb2f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bb2f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3bb2f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3bb2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bb2f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-116">Not supported.</span></span>|
|<span data-ttu-id="3bb2f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3bb2f-117">Application</span></span>|<span data-ttu-id="3bb2f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bb2f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3bb2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3bb2f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bb2f-120">Request headers</span></span>
|<span data-ttu-id="3bb2f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bb2f-121">Header</span></span>|<span data-ttu-id="3bb2f-122">値</span><span class="sxs-lookup"><span data-stu-id="3bb2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bb2f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bb2f-123">Authorization</span></span>|<span data-ttu-id="3bb2f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bb2f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3bb2f-125">Accept</span></span>|<span data-ttu-id="3bb2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3bb2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bb2f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3bb2f-127">Request body</span></span>
<span data-ttu-id="3bb2f-128">要求本文で、[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-128">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="3bb2f-129">次の表に、[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-129">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="3bb2f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3bb2f-130">Property</span></span>|<span data-ttu-id="3bb2f-131">型</span><span class="sxs-lookup"><span data-stu-id="3bb2f-131">Type</span></span>|<span data-ttu-id="3bb2f-132">説明</span><span class="sxs-lookup"><span data-stu-id="3bb2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bb2f-133">id</span><span class="sxs-lookup"><span data-stu-id="3bb2f-133">id</span></span>|<span data-ttu-id="3bb2f-134">String</span><span class="sxs-lookup"><span data-stu-id="3bb2f-134">String</span></span>|<span data-ttu-id="3bb2f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-135">Key of the entity.</span></span>|
|<span data-ttu-id="3bb2f-136">target</span><span class="sxs-lookup"><span data-stu-id="3bb2f-136">target</span></span>|[<span data-ttu-id="3bb2f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3bb2f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3bb2f-138">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="3bb2f-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="3bb2f-139">installIntent</span></span>|[<span data-ttu-id="3bb2f-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="3bb2f-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="3bb2f-141">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-141">The install intent for eBook.</span></span> <span data-ttu-id="3bb2f-142">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="3bb2f-143">応答</span><span class="sxs-lookup"><span data-stu-id="3bb2f-143">Response</span></span>
<span data-ttu-id="3bb2f-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-144">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bb2f-145">例</span><span class="sxs-lookup"><span data-stu-id="3bb2f-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bb2f-146">要求</span><span class="sxs-lookup"><span data-stu-id="3bb2f-146">Request</span></span>
<span data-ttu-id="3bb2f-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3bb2f-148">応答</span><span class="sxs-lookup"><span data-stu-id="3bb2f-148">Response</span></span>
<span data-ttu-id="3bb2f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3bb2f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




