---
title: mobileAppAssignment の作成
description: 新しい mobileAppAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3329b768e3e2151893b5886ed50d80b212e345f5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002070"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="0d443-103">mobileAppAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="0d443-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="0d443-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d443-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d443-105">新しい [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0d443-105">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d443-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="0d443-106">Prerequisites</span></span>
<span data-ttu-id="0d443-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d443-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d443-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0d443-109">Permission type</span></span>|<span data-ttu-id="0d443-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0d443-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d443-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0d443-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0d443-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d443-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0d443-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0d443-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d443-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d443-114">Not supported.</span></span>|
|<span data-ttu-id="0d443-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0d443-115">Application</span></span>|<span data-ttu-id="0d443-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d443-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d443-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0d443-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0d443-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d443-118">Request headers</span></span>
|<span data-ttu-id="0d443-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d443-119">Header</span></span>|<span data-ttu-id="0d443-120">値</span><span class="sxs-lookup"><span data-stu-id="0d443-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d443-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d443-121">Authorization</span></span>|<span data-ttu-id="0d443-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d443-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d443-123">承諾</span><span class="sxs-lookup"><span data-stu-id="0d443-123">Accept</span></span>|<span data-ttu-id="0d443-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0d443-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d443-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0d443-125">Request body</span></span>
<span data-ttu-id="0d443-126">要求本文で、mobileAppAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0d443-126">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="0d443-127">次の表に、mobileAppAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0d443-127">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="0d443-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d443-128">Property</span></span>|<span data-ttu-id="0d443-129">型</span><span class="sxs-lookup"><span data-stu-id="0d443-129">Type</span></span>|<span data-ttu-id="0d443-130">説明</span><span class="sxs-lookup"><span data-stu-id="0d443-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d443-131">id</span><span class="sxs-lookup"><span data-stu-id="0d443-131">id</span></span>|<span data-ttu-id="0d443-132">String</span><span class="sxs-lookup"><span data-stu-id="0d443-132">String</span></span>|<span data-ttu-id="0d443-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0d443-133">Key of the entity.</span></span>|
|<span data-ttu-id="0d443-134">intent</span><span class="sxs-lookup"><span data-stu-id="0d443-134">intent</span></span>|[<span data-ttu-id="0d443-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="0d443-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="0d443-136">管理者によって定義されたインストールの目的。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="0d443-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="0d443-137">target</span><span class="sxs-lookup"><span data-stu-id="0d443-137">target</span></span>|[<span data-ttu-id="0d443-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0d443-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0d443-139">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="0d443-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="0d443-140">settings</span><span class="sxs-lookup"><span data-stu-id="0d443-140">settings</span></span>|[<span data-ttu-id="0d443-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="0d443-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="0d443-142">管理者によって定義された、ターゲットの割り当ての設定。</span><span class="sxs-lookup"><span data-stu-id="0d443-142">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="0d443-143">応答</span><span class="sxs-lookup"><span data-stu-id="0d443-143">Response</span></span>
<span data-ttu-id="0d443-144">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0d443-144">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d443-145">例</span><span class="sxs-lookup"><span data-stu-id="0d443-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d443-146">要求</span><span class="sxs-lookup"><span data-stu-id="0d443-146">Request</span></span>
<span data-ttu-id="0d443-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0d443-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="0d443-148">応答</span><span class="sxs-lookup"><span data-stu-id="0d443-148">Response</span></span>
<span data-ttu-id="0d443-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0d443-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



