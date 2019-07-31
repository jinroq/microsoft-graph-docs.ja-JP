---
title: IntuneBrandingProfileAssignment を作成する
description: 新しい intuneBrandingProfileAssignment オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e0223a709a2b5be7a4d92de5ff3b27a807a389be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979219"
---
# <a name="create-intunebrandingprofileassignment"></a><span data-ttu-id="28e97-103">IntuneBrandingProfileAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="28e97-103">Create intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="28e97-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28e97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28e97-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="28e97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28e97-106">新しい[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="28e97-106">Create a new [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28e97-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="28e97-107">Prerequisites</span></span>
<span data-ttu-id="28e97-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28e97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28e97-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="28e97-110">Permission type</span></span>|<span data-ttu-id="28e97-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="28e97-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28e97-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="28e97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28e97-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28e97-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="28e97-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="28e97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28e97-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28e97-115">Not supported.</span></span>|
|<span data-ttu-id="28e97-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="28e97-116">Application</span></span>|<span data-ttu-id="28e97-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28e97-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28e97-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="28e97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="28e97-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28e97-119">Request headers</span></span>
|<span data-ttu-id="28e97-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28e97-120">Header</span></span>|<span data-ttu-id="28e97-121">値</span><span class="sxs-lookup"><span data-stu-id="28e97-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28e97-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28e97-122">Authorization</span></span>|<span data-ttu-id="28e97-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="28e97-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28e97-124">承諾</span><span class="sxs-lookup"><span data-stu-id="28e97-124">Accept</span></span>|<span data-ttu-id="28e97-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28e97-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28e97-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="28e97-126">Request body</span></span>
<span data-ttu-id="28e97-127">要求本文で、intuneBrandingProfileAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="28e97-127">In the request body, supply a JSON representation for the intuneBrandingProfileAssignment object.</span></span>

<span data-ttu-id="28e97-128">次の表に、intuneBrandingProfileAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="28e97-128">The following table shows the properties that are required when you create the intuneBrandingProfileAssignment.</span></span>

|<span data-ttu-id="28e97-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28e97-129">Property</span></span>|<span data-ttu-id="28e97-130">型</span><span class="sxs-lookup"><span data-stu-id="28e97-130">Type</span></span>|<span data-ttu-id="28e97-131">説明</span><span class="sxs-lookup"><span data-stu-id="28e97-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28e97-132">id</span><span class="sxs-lookup"><span data-stu-id="28e97-132">id</span></span>|<span data-ttu-id="28e97-133">String</span><span class="sxs-lookup"><span data-stu-id="28e97-133">String</span></span>|<span data-ttu-id="28e97-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="28e97-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="28e97-135">target</span><span class="sxs-lookup"><span data-stu-id="28e97-135">target</span></span>|[<span data-ttu-id="28e97-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="28e97-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="28e97-137">ブランド化プロファイルが割り当てられている割り当て先。</span><span class="sxs-lookup"><span data-stu-id="28e97-137">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="28e97-138">応答</span><span class="sxs-lookup"><span data-stu-id="28e97-138">Response</span></span>
<span data-ttu-id="28e97-139">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="28e97-139">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28e97-140">例</span><span class="sxs-lookup"><span data-stu-id="28e97-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="28e97-141">要求</span><span class="sxs-lookup"><span data-stu-id="28e97-141">Request</span></span>
<span data-ttu-id="28e97-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="28e97-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
Content-type: application/json
Content-length: 171

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="28e97-143">応答</span><span class="sxs-lookup"><span data-stu-id="28e97-143">Response</span></span>
<span data-ttu-id="28e97-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="28e97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





