---
title: mobileAppAssignment の作成
description: 新しい mobileAppAssignment オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 94fb6e79077e687df11cda4b28b71b8e97360971
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397982"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="9d4fd-103">mobileAppAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="9d4fd-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="9d4fd-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9d4fd-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d4fd-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d4fd-107">新しい [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d4fd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9d4fd-108">Prerequisites</span></span>
<span data-ttu-id="9d4fd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9d4fd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d4fd-111">Permission type</span></span>|<span data-ttu-id="9d4fd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d4fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d4fd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d4fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d4fd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d4fd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9d4fd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d4fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d4fd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-116">Not supported.</span></span>|
|<span data-ttu-id="9d4fd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d4fd-117">Application</span></span>|<span data-ttu-id="9d4fd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d4fd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d4fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9d4fd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d4fd-120">Request headers</span></span>
|<span data-ttu-id="9d4fd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d4fd-121">Header</span></span>|<span data-ttu-id="9d4fd-122">値</span><span class="sxs-lookup"><span data-stu-id="9d4fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d4fd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d4fd-123">Authorization</span></span>|<span data-ttu-id="9d4fd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d4fd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9d4fd-125">Accept</span></span>|<span data-ttu-id="9d4fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d4fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d4fd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d4fd-127">Request body</span></span>
<span data-ttu-id="9d4fd-128">要求本文で、mobileAppAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="9d4fd-129">次の表に、mobileAppAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="9d4fd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d4fd-130">Property</span></span>|<span data-ttu-id="9d4fd-131">型</span><span class="sxs-lookup"><span data-stu-id="9d4fd-131">Type</span></span>|<span data-ttu-id="9d4fd-132">説明</span><span class="sxs-lookup"><span data-stu-id="9d4fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d4fd-133">id</span><span class="sxs-lookup"><span data-stu-id="9d4fd-133">id</span></span>|<span data-ttu-id="9d4fd-134">String</span><span class="sxs-lookup"><span data-stu-id="9d4fd-134">String</span></span>|<span data-ttu-id="9d4fd-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-135">Key of the entity.</span></span>|
|<span data-ttu-id="9d4fd-136">intent</span><span class="sxs-lookup"><span data-stu-id="9d4fd-136">intent</span></span>|[<span data-ttu-id="9d4fd-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="9d4fd-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="9d4fd-138">管理者によって定義されたインストールの目的。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="9d4fd-139">target</span><span class="sxs-lookup"><span data-stu-id="9d4fd-139">target</span></span>|[<span data-ttu-id="9d4fd-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9d4fd-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9d4fd-141">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="9d4fd-142">settings</span><span class="sxs-lookup"><span data-stu-id="9d4fd-142">settings</span></span>|[<span data-ttu-id="9d4fd-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="9d4fd-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="9d4fd-144">管理者によって定義された、ターゲットの割り当ての設定。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="9d4fd-145">応答</span><span class="sxs-lookup"><span data-stu-id="9d4fd-145">Response</span></span>
<span data-ttu-id="9d4fd-146">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-146">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d4fd-147">例</span><span class="sxs-lookup"><span data-stu-id="9d4fd-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d4fd-148">要求</span><span class="sxs-lookup"><span data-stu-id="9d4fd-148">Request</span></span>
<span data-ttu-id="9d4fd-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
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

### <a name="response"></a><span data-ttu-id="9d4fd-150">応答</span><span class="sxs-lookup"><span data-stu-id="9d4fd-150">Response</span></span>
<span data-ttu-id="9d4fd-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




