---
title: deviceConfigurationConflictSummary の更新
description: deviceConfigurationConflictSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a86283e088a4ef28beb1c0139d3650877ed0d651
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32470441"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="a0d10-103">deviceConfigurationConflictSummary の更新</span><span class="sxs-lookup"><span data-stu-id="a0d10-103">Update deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="a0d10-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0d10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0d10-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a0d10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0d10-106">[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a0d10-106">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0d10-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a0d10-107">Prerequisites</span></span>
<span data-ttu-id="a0d10-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a0d10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0d10-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a0d10-110">Permission type</span></span>|<span data-ttu-id="a0d10-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a0d10-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0d10-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a0d10-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0d10-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0d10-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0d10-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a0d10-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0d10-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0d10-115">Not supported.</span></span>|
|<span data-ttu-id="a0d10-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a0d10-116">Application</span></span>|<span data-ttu-id="a0d10-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0d10-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0d10-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a0d10-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="a0d10-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a0d10-119">Request headers</span></span>
|<span data-ttu-id="a0d10-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a0d10-120">Header</span></span>|<span data-ttu-id="a0d10-121">値</span><span class="sxs-lookup"><span data-stu-id="a0d10-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0d10-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0d10-122">Authorization</span></span>|<span data-ttu-id="a0d10-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a0d10-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0d10-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a0d10-124">Accept</span></span>|<span data-ttu-id="a0d10-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0d10-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0d10-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a0d10-126">Request body</span></span>
<span data-ttu-id="a0d10-127">要求本文で、 [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a0d10-127">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="a0d10-128">次の表に、 [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a0d10-128">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="a0d10-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0d10-129">Property</span></span>|<span data-ttu-id="a0d10-130">型</span><span class="sxs-lookup"><span data-stu-id="a0d10-130">Type</span></span>|<span data-ttu-id="a0d10-131">説明</span><span class="sxs-lookup"><span data-stu-id="a0d10-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0d10-132">競合する devicdeviceconfigurん</span><span class="sxs-lookup"><span data-stu-id="a0d10-132">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="a0d10-133">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a0d10-133">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="a0d10-134">指定された設定と競合しているポリシーのセット</span><span class="sxs-lookup"><span data-stu-id="a0d10-134">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="a0d10-135">id</span><span class="sxs-lookup"><span data-stu-id="a0d10-135">id</span></span>|<span data-ttu-id="a0d10-136">String</span><span class="sxs-lookup"><span data-stu-id="a0d10-136">String</span></span>|<span data-ttu-id="a0d10-137">競合しているポリシーのセットの id。</span><span class="sxs-lookup"><span data-stu-id="a0d10-137">The id for this set of conflicting policies.</span></span> <span data-ttu-id="a0d10-138">この id は、アンダースコアで区切られた辞書順で競合しているすべてのポリシーの id です。</span><span class="sxs-lookup"><span data-stu-id="a0d10-138">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="a0d10-139">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="a0d10-139">contributingSettings</span></span>|<span data-ttu-id="a0d10-140">String collection</span><span class="sxs-lookup"><span data-stu-id="a0d10-140">String collection</span></span>|<span data-ttu-id="a0d10-141">指定されたポリシーと競合する設定のセット</span><span class="sxs-lookup"><span data-stu-id="a0d10-141">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="a0d10-142">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="a0d10-142">deviceCheckinsImpacted</span></span>|<span data-ttu-id="a0d10-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a0d10-143">Int32</span></span>|<span data-ttu-id="a0d10-144">競合するポリシーと設定によって影響を受けるチェックインの数</span><span class="sxs-lookup"><span data-stu-id="a0d10-144">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="a0d10-145">応答</span><span class="sxs-lookup"><span data-stu-id="a0d10-145">Response</span></span>
<span data-ttu-id="a0d10-146">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a0d10-146">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0d10-147">例</span><span class="sxs-lookup"><span data-stu-id="a0d10-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0d10-148">要求</span><span class="sxs-lookup"><span data-stu-id="a0d10-148">Request</span></span>
<span data-ttu-id="a0d10-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a0d10-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```

### <a name="response"></a><span data-ttu-id="a0d10-150">応答</span><span class="sxs-lookup"><span data-stu-id="a0d10-150">Response</span></span>
<span data-ttu-id="a0d10-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a0d10-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 410

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```





