---
title: mobileAppAssignment の作成
description: 新しい mobileAppAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8feb99e520e159b1aeba14d14fd40331201209b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576046"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="ce79e-103">mobileAppAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="ce79e-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="ce79e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce79e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce79e-105">新しい [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ce79e-105">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce79e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ce79e-106">Prerequisites</span></span>
<span data-ttu-id="ce79e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce79e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce79e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce79e-109">Permission type</span></span>|<span data-ttu-id="ce79e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce79e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce79e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce79e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ce79e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce79e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce79e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce79e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce79e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce79e-114">Not supported.</span></span>|
|<span data-ttu-id="ce79e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce79e-115">Application</span></span>|<span data-ttu-id="ce79e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce79e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce79e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce79e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ce79e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce79e-118">Request headers</span></span>
|<span data-ttu-id="ce79e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce79e-119">Header</span></span>|<span data-ttu-id="ce79e-120">値</span><span class="sxs-lookup"><span data-stu-id="ce79e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce79e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce79e-121">Authorization</span></span>|<span data-ttu-id="ce79e-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce79e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce79e-123">承諾</span><span class="sxs-lookup"><span data-stu-id="ce79e-123">Accept</span></span>|<span data-ttu-id="ce79e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ce79e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce79e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce79e-125">Request body</span></span>
<span data-ttu-id="ce79e-126">要求本文で、mobileAppAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce79e-126">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="ce79e-127">次の表に、mobileAppAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ce79e-127">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="ce79e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce79e-128">Property</span></span>|<span data-ttu-id="ce79e-129">型</span><span class="sxs-lookup"><span data-stu-id="ce79e-129">Type</span></span>|<span data-ttu-id="ce79e-130">説明</span><span class="sxs-lookup"><span data-stu-id="ce79e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce79e-131">id</span><span class="sxs-lookup"><span data-stu-id="ce79e-131">id</span></span>|<span data-ttu-id="ce79e-132">String</span><span class="sxs-lookup"><span data-stu-id="ce79e-132">String</span></span>|<span data-ttu-id="ce79e-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ce79e-133">Key of the entity.</span></span>|
|<span data-ttu-id="ce79e-134">intent</span><span class="sxs-lookup"><span data-stu-id="ce79e-134">intent</span></span>|[<span data-ttu-id="ce79e-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="ce79e-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="ce79e-136">管理者によって定義されたインストールの目的。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="ce79e-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="ce79e-137">target</span><span class="sxs-lookup"><span data-stu-id="ce79e-137">target</span></span>|[<span data-ttu-id="ce79e-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ce79e-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ce79e-139">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="ce79e-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="ce79e-140">settings</span><span class="sxs-lookup"><span data-stu-id="ce79e-140">settings</span></span>|[<span data-ttu-id="ce79e-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ce79e-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="ce79e-142">管理者によって定義された、ターゲットの割り当ての設定。</span><span class="sxs-lookup"><span data-stu-id="ce79e-142">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="ce79e-143">応答</span><span class="sxs-lookup"><span data-stu-id="ce79e-143">Response</span></span>
<span data-ttu-id="ce79e-144">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ce79e-144">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce79e-145">例</span><span class="sxs-lookup"><span data-stu-id="ce79e-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce79e-146">要求</span><span class="sxs-lookup"><span data-stu-id="ce79e-146">Request</span></span>
<span data-ttu-id="ce79e-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce79e-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ce79e-148">応答</span><span class="sxs-lookup"><span data-stu-id="ce79e-148">Response</span></span>
<span data-ttu-id="ce79e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ce79e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



