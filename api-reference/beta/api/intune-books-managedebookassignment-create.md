---
title: managedEBookAssignment の作成
description: 新しい managedEBookAssignment オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f1f00c4db40b157359fd04171df6799d56949caa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409560"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="4b599-103">managedEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="4b599-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="4b599-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4b599-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4b599-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b599-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b599-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4b599-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b599-107">新しい [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4b599-107">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b599-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4b599-108">Prerequisites</span></span>
<span data-ttu-id="4b599-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4b599-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4b599-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4b599-111">Permission type</span></span>|<span data-ttu-id="4b599-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4b599-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b599-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4b599-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b599-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b599-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4b599-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4b599-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b599-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b599-116">Not supported.</span></span>|
|<span data-ttu-id="4b599-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4b599-117">Application</span></span>|<span data-ttu-id="4b599-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b599-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b599-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4b599-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4b599-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b599-120">Request headers</span></span>
|<span data-ttu-id="4b599-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b599-121">Header</span></span>|<span data-ttu-id="4b599-122">値</span><span class="sxs-lookup"><span data-stu-id="4b599-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b599-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b599-123">Authorization</span></span>|<span data-ttu-id="4b599-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4b599-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b599-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b599-125">Accept</span></span>|<span data-ttu-id="4b599-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b599-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b599-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4b599-127">Request body</span></span>
<span data-ttu-id="4b599-128">要求本文で、managedEBookAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4b599-128">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="4b599-129">次の表に、managedEBookAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4b599-129">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="4b599-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b599-130">Property</span></span>|<span data-ttu-id="4b599-131">型</span><span class="sxs-lookup"><span data-stu-id="4b599-131">Type</span></span>|<span data-ttu-id="4b599-132">説明</span><span class="sxs-lookup"><span data-stu-id="4b599-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b599-133">id</span><span class="sxs-lookup"><span data-stu-id="4b599-133">id</span></span>|<span data-ttu-id="4b599-134">String</span><span class="sxs-lookup"><span data-stu-id="4b599-134">String</span></span>|<span data-ttu-id="4b599-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4b599-135">Key of the entity.</span></span>|
|<span data-ttu-id="4b599-136">target</span><span class="sxs-lookup"><span data-stu-id="4b599-136">target</span></span>|[<span data-ttu-id="4b599-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4b599-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4b599-138">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="4b599-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="4b599-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="4b599-139">installIntent</span></span>|[<span data-ttu-id="4b599-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="4b599-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="4b599-141">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="4b599-141">The install intent for eBook.</span></span> <span data-ttu-id="4b599-142">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="4b599-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="4b599-143">応答</span><span class="sxs-lookup"><span data-stu-id="4b599-143">Response</span></span>
<span data-ttu-id="4b599-144">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4b599-144">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b599-145">例</span><span class="sxs-lookup"><span data-stu-id="4b599-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b599-146">要求</span><span class="sxs-lookup"><span data-stu-id="4b599-146">Request</span></span>
<span data-ttu-id="4b599-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4b599-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4b599-148">応答</span><span class="sxs-lookup"><span data-stu-id="4b599-148">Response</span></span>
<span data-ttu-id="4b599-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4b599-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




