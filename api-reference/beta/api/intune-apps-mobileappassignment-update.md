---
title: mobileAppAssignment の更新
description: mobileAppAssignment オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b56df8300d7c96bbb5ab3aea24716592922069f5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974126"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="65269-103">mobileAppAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="65269-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="65269-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65269-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65269-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="65269-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65269-106">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="65269-106">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65269-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="65269-107">Prerequisites</span></span>
<span data-ttu-id="65269-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65269-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65269-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65269-110">Permission type</span></span>|<span data-ttu-id="65269-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="65269-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65269-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65269-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65269-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65269-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="65269-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65269-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65269-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65269-115">Not supported.</span></span>|
|<span data-ttu-id="65269-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65269-116">Application</span></span>|<span data-ttu-id="65269-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65269-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65269-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65269-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="65269-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65269-119">Request headers</span></span>
|<span data-ttu-id="65269-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65269-120">Header</span></span>|<span data-ttu-id="65269-121">値</span><span class="sxs-lookup"><span data-stu-id="65269-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65269-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65269-122">Authorization</span></span>|<span data-ttu-id="65269-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="65269-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65269-124">承諾</span><span class="sxs-lookup"><span data-stu-id="65269-124">Accept</span></span>|<span data-ttu-id="65269-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65269-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65269-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="65269-126">Request body</span></span>
<span data-ttu-id="65269-127">要求本文で、[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="65269-127">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="65269-128">次の表に、[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="65269-128">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="65269-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65269-129">Property</span></span>|<span data-ttu-id="65269-130">型</span><span class="sxs-lookup"><span data-stu-id="65269-130">Type</span></span>|<span data-ttu-id="65269-131">説明</span><span class="sxs-lookup"><span data-stu-id="65269-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65269-132">id</span><span class="sxs-lookup"><span data-stu-id="65269-132">id</span></span>|<span data-ttu-id="65269-133">String</span><span class="sxs-lookup"><span data-stu-id="65269-133">String</span></span>|<span data-ttu-id="65269-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="65269-134">Key of the entity.</span></span>|
|<span data-ttu-id="65269-135">intent</span><span class="sxs-lookup"><span data-stu-id="65269-135">intent</span></span>|[<span data-ttu-id="65269-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="65269-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="65269-137">管理者によって定義されたインストールの目的。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="65269-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="65269-138">target</span><span class="sxs-lookup"><span data-stu-id="65269-138">target</span></span>|[<span data-ttu-id="65269-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="65269-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="65269-140">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="65269-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="65269-141">settings</span><span class="sxs-lookup"><span data-stu-id="65269-141">settings</span></span>|[<span data-ttu-id="65269-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="65269-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="65269-143">管理者によって定義された、ターゲットの割り当ての設定。</span><span class="sxs-lookup"><span data-stu-id="65269-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="65269-144">応答</span><span class="sxs-lookup"><span data-stu-id="65269-144">Response</span></span>
<span data-ttu-id="65269-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="65269-145">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65269-146">例</span><span class="sxs-lookup"><span data-stu-id="65269-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="65269-147">要求</span><span class="sxs-lookup"><span data-stu-id="65269-147">Request</span></span>
<span data-ttu-id="65269-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="65269-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
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

### <a name="response"></a><span data-ttu-id="65269-149">応答</span><span class="sxs-lookup"><span data-stu-id="65269-149">Response</span></span>
<span data-ttu-id="65269-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="65269-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





