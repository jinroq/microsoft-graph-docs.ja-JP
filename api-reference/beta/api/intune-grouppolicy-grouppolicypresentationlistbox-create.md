---
title: GroupPolicyPresentationListBox の作成
description: 新しい groupPolicyPresentationListBox オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5de84a8867e14737611b6d10ab7d2c69159e22b2
ms.sourcegitcommit: 705b32b9a64516d8138fab34c173b7df4f78a6ad
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/05/2019
ms.locfileid: "35576474"
---
# <a name="create-grouppolicypresentationlistbox"></a><span data-ttu-id="7c44c-103">GroupPolicyPresentationListBox の作成</span><span class="sxs-lookup"><span data-stu-id="7c44c-103">Create groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="7c44c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c44c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c44c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7c44c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c44c-106">新しい[Grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7c44c-106">Create a new [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c44c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7c44c-107">Prerequisites</span></span>
<span data-ttu-id="7c44c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c44c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c44c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c44c-110">Permission type</span></span>|<span data-ttu-id="7c44c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c44c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c44c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c44c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c44c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c44c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7c44c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c44c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c44c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c44c-115">Not supported.</span></span>|
|<span data-ttu-id="7c44c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c44c-116">Application</span></span>|<span data-ttu-id="7c44c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c44c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c44c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c44c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="7c44c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c44c-119">Request headers</span></span>
|<span data-ttu-id="7c44c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c44c-120">Header</span></span>|<span data-ttu-id="7c44c-121">値</span><span class="sxs-lookup"><span data-stu-id="7c44c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c44c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c44c-122">Authorization</span></span>|<span data-ttu-id="7c44c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7c44c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c44c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7c44c-124">Accept</span></span>|<span data-ttu-id="7c44c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c44c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c44c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c44c-126">Request body</span></span>
<span data-ttu-id="7c44c-127">要求本文で、groupPolicyPresentationListBox オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c44c-127">In the request body, supply a JSON representation for the groupPolicyPresentationListBox object.</span></span>

<span data-ttu-id="7c44c-128">次の表に、groupPolicyPresentationListBox の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7c44c-128">The following table shows the properties that are required when you create the groupPolicyPresentationListBox.</span></span>

|<span data-ttu-id="7c44c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c44c-129">Property</span></span>|<span data-ttu-id="7c44c-130">型</span><span class="sxs-lookup"><span data-stu-id="7c44c-130">Type</span></span>|<span data-ttu-id="7c44c-131">説明</span><span class="sxs-lookup"><span data-stu-id="7c44c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c44c-132">label</span><span class="sxs-lookup"><span data-stu-id="7c44c-132">label</span></span>|<span data-ttu-id="7c44c-133">String</span><span class="sxs-lookup"><span data-stu-id="7c44c-133">String</span></span>|<span data-ttu-id="7c44c-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="7c44c-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="7c44c-135">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="7c44c-135">The default value is empty.</span></span> <span data-ttu-id="7c44c-136">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7c44c-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7c44c-137">id</span><span class="sxs-lookup"><span data-stu-id="7c44c-137">id</span></span>|<span data-ttu-id="7c44c-138">String</span><span class="sxs-lookup"><span data-stu-id="7c44c-138">String</span></span>|<span data-ttu-id="7c44c-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7c44c-139">Key of the entity.</span></span> <span data-ttu-id="7c44c-140">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7c44c-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7c44c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c44c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="7c44c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c44c-142">DateTimeOffset</span></span>|<span data-ttu-id="7c44c-143">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="7c44c-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="7c44c-144">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7c44c-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7c44c-145">explicitValue</span><span class="sxs-lookup"><span data-stu-id="7c44c-145">explicitValue</span></span>|<span data-ttu-id="7c44c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c44c-146">Boolean</span></span>|<span data-ttu-id="7c44c-147">このオプションが指定されている場合、ユーザーはレジストリサブキーの値とレジストリサブキー名を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c44c-147">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="7c44c-148">リストボックスに2つの列が表示されます。1つは名前用、もう1つはデータ用です。</span><span class="sxs-lookup"><span data-stu-id="7c44c-148">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="7c44c-149">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="7c44c-149">The default value is false.</span></span>|
|<span data-ttu-id="7c44c-150">valuePrefix</span><span class="sxs-lookup"><span data-stu-id="7c44c-150">valuePrefix</span></span>|<span data-ttu-id="7c44c-151">String</span><span class="sxs-lookup"><span data-stu-id="7c44c-151">String</span></span>|<span data-ttu-id="7c44c-152">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7c44c-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7c44c-153">応答</span><span class="sxs-lookup"><span data-stu-id="7c44c-153">Response</span></span>
<span data-ttu-id="7c44c-154">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7c44c-154">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c44c-155">例</span><span class="sxs-lookup"><span data-stu-id="7c44c-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c44c-156">要求</span><span class="sxs-lookup"><span data-stu-id="7c44c-156">Request</span></span>
<span data-ttu-id="7c44c-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7c44c-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true,
  "valuePrefix": "Value Prefix value"
}
```

### <a name="response"></a><span data-ttu-id="7c44c-158">応答</span><span class="sxs-lookup"><span data-stu-id="7c44c-158">Response</span></span>
<span data-ttu-id="7c44c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7c44c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "id": "2e074c87-4c87-2e07-874c-072e874c072e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "explicitValue": true,
  "valuePrefix": "Value Prefix value"
}
```



