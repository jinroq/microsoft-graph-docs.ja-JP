---
title: intuneBrandingProfileAssignment の更新
description: intuneBrandingProfileAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16b49bd41ed0ce612b1d481553386cc8f789e187
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541781"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="5b975-103">intuneBrandingProfileAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="5b975-103">Update intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="5b975-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b975-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b975-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5b975-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b975-106">[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5b975-106">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b975-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5b975-107">Prerequisites</span></span>
<span data-ttu-id="5b975-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b975-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b975-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b975-110">Permission type</span></span>|<span data-ttu-id="5b975-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b975-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b975-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b975-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b975-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b975-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5b975-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b975-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b975-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b975-115">Not supported.</span></span>|
|<span data-ttu-id="5b975-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b975-116">Application</span></span>|<span data-ttu-id="5b975-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b975-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b975-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b975-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5b975-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b975-119">Request headers</span></span>
|<span data-ttu-id="5b975-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b975-120">Header</span></span>|<span data-ttu-id="5b975-121">値</span><span class="sxs-lookup"><span data-stu-id="5b975-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b975-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b975-122">Authorization</span></span>|<span data-ttu-id="5b975-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5b975-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b975-124">承諾</span><span class="sxs-lookup"><span data-stu-id="5b975-124">Accept</span></span>|<span data-ttu-id="5b975-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b975-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b975-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b975-126">Request body</span></span>
<span data-ttu-id="5b975-127">要求本文で、 [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5b975-127">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="5b975-128">次の表に、 [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5b975-128">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="5b975-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b975-129">Property</span></span>|<span data-ttu-id="5b975-130">型</span><span class="sxs-lookup"><span data-stu-id="5b975-130">Type</span></span>|<span data-ttu-id="5b975-131">説明</span><span class="sxs-lookup"><span data-stu-id="5b975-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b975-132">id</span><span class="sxs-lookup"><span data-stu-id="5b975-132">id</span></span>|<span data-ttu-id="5b975-133">String</span><span class="sxs-lookup"><span data-stu-id="5b975-133">String</span></span>|<span data-ttu-id="5b975-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5b975-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="5b975-135">target</span><span class="sxs-lookup"><span data-stu-id="5b975-135">target</span></span>|[<span data-ttu-id="5b975-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5b975-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5b975-137">ブランド化プロファイルが割り当てられている割り当て先。</span><span class="sxs-lookup"><span data-stu-id="5b975-137">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="5b975-138">応答</span><span class="sxs-lookup"><span data-stu-id="5b975-138">Response</span></span>
<span data-ttu-id="5b975-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5b975-139">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b975-140">例</span><span class="sxs-lookup"><span data-stu-id="5b975-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b975-141">要求</span><span class="sxs-lookup"><span data-stu-id="5b975-141">Request</span></span>
<span data-ttu-id="5b975-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5b975-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b975-143">応答</span><span class="sxs-lookup"><span data-stu-id="5b975-143">Response</span></span>
<span data-ttu-id="5b975-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5b975-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





