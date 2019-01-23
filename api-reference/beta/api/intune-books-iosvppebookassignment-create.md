---
title: iosVppEBookAssignment の作成
description: 新しい iosVppEBookAssignment オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3cfebd4f1b61ae7cfc3c4a92d2c3415ce18e4cab
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424505"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="538b0-103">iosVppEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="538b0-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="538b0-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="538b0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="538b0-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="538b0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="538b0-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="538b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="538b0-107">新しい [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="538b0-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="538b0-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="538b0-108">Prerequisites</span></span>
<span data-ttu-id="538b0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="538b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="538b0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="538b0-111">Permission type</span></span>|<span data-ttu-id="538b0-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="538b0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="538b0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="538b0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="538b0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="538b0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="538b0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="538b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="538b0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="538b0-116">Not supported.</span></span>|
|<span data-ttu-id="538b0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="538b0-117">Application</span></span>|<span data-ttu-id="538b0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="538b0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="538b0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="538b0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="538b0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="538b0-120">Request headers</span></span>
|<span data-ttu-id="538b0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="538b0-121">Header</span></span>|<span data-ttu-id="538b0-122">値</span><span class="sxs-lookup"><span data-stu-id="538b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="538b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="538b0-123">Authorization</span></span>|<span data-ttu-id="538b0-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="538b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="538b0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="538b0-125">Accept</span></span>|<span data-ttu-id="538b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="538b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="538b0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="538b0-127">Request body</span></span>
<span data-ttu-id="538b0-128">要求本文で、iosVppEBookAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="538b0-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="538b0-129">次の表に、iosVppEBookAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="538b0-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="538b0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="538b0-130">Property</span></span>|<span data-ttu-id="538b0-131">型</span><span class="sxs-lookup"><span data-stu-id="538b0-131">Type</span></span>|<span data-ttu-id="538b0-132">説明</span><span class="sxs-lookup"><span data-stu-id="538b0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="538b0-133">id</span><span class="sxs-lookup"><span data-stu-id="538b0-133">id</span></span>|<span data-ttu-id="538b0-134">String</span><span class="sxs-lookup"><span data-stu-id="538b0-134">String</span></span>|<span data-ttu-id="538b0-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="538b0-135">Key of the entity.</span></span> <span data-ttu-id="538b0-136">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="538b0-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="538b0-137">target</span><span class="sxs-lookup"><span data-stu-id="538b0-137">target</span></span>|[<span data-ttu-id="538b0-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="538b0-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="538b0-139">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="538b0-139">The assignment target for eBook.</span></span> <span data-ttu-id="538b0-140">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="538b0-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="538b0-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="538b0-141">installIntent</span></span>|[<span data-ttu-id="538b0-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="538b0-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="538b0-143">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="538b0-143">The install intent for eBook.</span></span> <span data-ttu-id="538b0-144">[ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="538b0-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="538b0-145">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="538b0-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="538b0-146">応答</span><span class="sxs-lookup"><span data-stu-id="538b0-146">Response</span></span>
<span data-ttu-id="538b0-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="538b0-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="538b0-148">例</span><span class="sxs-lookup"><span data-stu-id="538b0-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="538b0-149">要求</span><span class="sxs-lookup"><span data-stu-id="538b0-149">Request</span></span>
<span data-ttu-id="538b0-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="538b0-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="538b0-151">応答</span><span class="sxs-lookup"><span data-stu-id="538b0-151">Response</span></span>
<span data-ttu-id="538b0-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="538b0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




