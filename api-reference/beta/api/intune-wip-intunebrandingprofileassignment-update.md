---
title: IntuneBrandingProfileAssignment を更新します。
description: IntuneBrandingProfileAssignment オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7bfdba766221fc27dde6a8b71212620b744c4fc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430291"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="d5c1f-103">IntuneBrandingProfileAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-103">Update intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="d5c1f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d5c1f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5c1f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5c1f-107">[IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-107">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5c1f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d5c1f-108">Prerequisites</span></span>
<span data-ttu-id="d5c1f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d5c1f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5c1f-111">Permission type</span></span>|<span data-ttu-id="d5c1f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5c1f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5c1f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5c1f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5c1f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5c1f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d5c1f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5c1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5c1f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-116">Not supported.</span></span>|
|<span data-ttu-id="d5c1f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5c1f-117">Application</span></span>|<span data-ttu-id="d5c1f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5c1f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5c1f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d5c1f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5c1f-120">Request headers</span></span>
|<span data-ttu-id="d5c1f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5c1f-121">Header</span></span>|<span data-ttu-id="d5c1f-122">値</span><span class="sxs-lookup"><span data-stu-id="d5c1f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5c1f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5c1f-123">Authorization</span></span>|<span data-ttu-id="d5c1f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5c1f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5c1f-125">Accept</span></span>|<span data-ttu-id="d5c1f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5c1f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5c1f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5c1f-127">Request body</span></span>
<span data-ttu-id="d5c1f-128">要求の本文に[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-128">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="d5c1f-129">[IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-129">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="d5c1f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5c1f-130">Property</span></span>|<span data-ttu-id="d5c1f-131">型</span><span class="sxs-lookup"><span data-stu-id="d5c1f-131">Type</span></span>|<span data-ttu-id="d5c1f-132">説明</span><span class="sxs-lookup"><span data-stu-id="d5c1f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5c1f-133">id</span><span class="sxs-lookup"><span data-stu-id="d5c1f-133">id</span></span>|<span data-ttu-id="d5c1f-134">String</span><span class="sxs-lookup"><span data-stu-id="d5c1f-134">String</span></span>|<span data-ttu-id="d5c1f-135">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d5c1f-136">target</span><span class="sxs-lookup"><span data-stu-id="d5c1f-136">target</span></span>|[<span data-ttu-id="d5c1f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d5c1f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d5c1f-138">割り当てのターゲットにブランドのプロファイルが割り当てられています。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="d5c1f-139">応答</span><span class="sxs-lookup"><span data-stu-id="d5c1f-139">Response</span></span>
<span data-ttu-id="d5c1f-140">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-140">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5c1f-141">例</span><span class="sxs-lookup"><span data-stu-id="d5c1f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5c1f-142">要求</span><span class="sxs-lookup"><span data-stu-id="d5c1f-142">Request</span></span>
<span data-ttu-id="d5c1f-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
Content-type: application/json
Content-length: 171

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d5c1f-144">応答</span><span class="sxs-lookup"><span data-stu-id="d5c1f-144">Response</span></span>
<span data-ttu-id="d5c1f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d5c1f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 220

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




