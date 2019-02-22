---
title: mobileAppAssignment の作成
description: 新しい mobileAppAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7abf1163d5d323bf460b0a8dab3b54eb7ef8a2f8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156701"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="028d5-103">mobileAppAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="028d5-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="028d5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="028d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="028d5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="028d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="028d5-106">新しい [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="028d5-106">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="028d5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="028d5-107">Prerequisites</span></span>
<span data-ttu-id="028d5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="028d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="028d5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="028d5-110">Permission type</span></span>|<span data-ttu-id="028d5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="028d5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="028d5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="028d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="028d5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="028d5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="028d5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="028d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="028d5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="028d5-115">Not supported.</span></span>|
|<span data-ttu-id="028d5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="028d5-116">Application</span></span>|<span data-ttu-id="028d5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="028d5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="028d5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="028d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="028d5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="028d5-119">Request headers</span></span>
|<span data-ttu-id="028d5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="028d5-120">Header</span></span>|<span data-ttu-id="028d5-121">値</span><span class="sxs-lookup"><span data-stu-id="028d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="028d5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="028d5-122">Authorization</span></span>|<span data-ttu-id="028d5-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="028d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="028d5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="028d5-124">Accept</span></span>|<span data-ttu-id="028d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="028d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="028d5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="028d5-126">Request body</span></span>
<span data-ttu-id="028d5-127">要求本文で、mobileAppAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="028d5-127">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="028d5-128">次の表に、mobileAppAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="028d5-128">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="028d5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="028d5-129">Property</span></span>|<span data-ttu-id="028d5-130">型</span><span class="sxs-lookup"><span data-stu-id="028d5-130">Type</span></span>|<span data-ttu-id="028d5-131">説明</span><span class="sxs-lookup"><span data-stu-id="028d5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="028d5-132">id</span><span class="sxs-lookup"><span data-stu-id="028d5-132">id</span></span>|<span data-ttu-id="028d5-133">String</span><span class="sxs-lookup"><span data-stu-id="028d5-133">String</span></span>|<span data-ttu-id="028d5-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="028d5-134">Key of the entity.</span></span>|
|<span data-ttu-id="028d5-135">intent</span><span class="sxs-lookup"><span data-stu-id="028d5-135">intent</span></span>|[<span data-ttu-id="028d5-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="028d5-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="028d5-137">管理者によって定義されたインストールの目的。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="028d5-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="028d5-138">target</span><span class="sxs-lookup"><span data-stu-id="028d5-138">target</span></span>|[<span data-ttu-id="028d5-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="028d5-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="028d5-140">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="028d5-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="028d5-141">settings</span><span class="sxs-lookup"><span data-stu-id="028d5-141">settings</span></span>|[<span data-ttu-id="028d5-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="028d5-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="028d5-143">管理者によって定義された、ターゲットの割り当ての設定。</span><span class="sxs-lookup"><span data-stu-id="028d5-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="028d5-144">応答</span><span class="sxs-lookup"><span data-stu-id="028d5-144">Response</span></span>
<span data-ttu-id="028d5-145">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="028d5-145">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="028d5-146">例</span><span class="sxs-lookup"><span data-stu-id="028d5-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="028d5-147">要求</span><span class="sxs-lookup"><span data-stu-id="028d5-147">Request</span></span>
<span data-ttu-id="028d5-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="028d5-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="028d5-149">応答</span><span class="sxs-lookup"><span data-stu-id="028d5-149">Response</span></span>
<span data-ttu-id="028d5-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="028d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




