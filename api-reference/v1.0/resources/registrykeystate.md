# <a name="registrykeystate-resource-type"></a><span data-ttu-id="81cf0-101">registryKeyState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="81cf0-101">registryKeyState resource type</span></span>

<span data-ttu-id="81cf0-102">アラート、およびレジストリ キーを変更するプロセスに関連するレジストリ キーの変更に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="81cf0-102">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="81cf0-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81cf0-103">Properties</span></span>

| <span data-ttu-id="81cf0-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81cf0-104">Property</span></span>     | <span data-ttu-id="81cf0-105">型</span><span class="sxs-lookup"><span data-stu-id="81cf0-105">Type</span></span>        | <span data-ttu-id="81cf0-106">説明</span><span class="sxs-lookup"><span data-stu-id="81cf0-106">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="81cf0-107">ハイブ</span><span class="sxs-lookup"><span data-stu-id="81cf0-107">Hive</span></span>|<span data-ttu-id="81cf0-108">registryHive</span><span class="sxs-lookup"><span data-stu-id="81cf0-108">registryHive</span></span>|<span data-ttu-id="81cf0-109">A [ Windows レジストリ ハイブ](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives)  :</span><span class="sxs-lookup"><span data-stu-id="81cf0-109">A [Windows registry hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="81cf0-110">HKEY_CURRENT_CONFIG ハイブです。</span><span class="sxs-lookup"><span data-stu-id="81cf0-110">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="81cf0-111">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="81cf0-111">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="81cf0-112">HKEY_LOCAL_MACHINE\SAM ハイブです。</span><span class="sxs-lookup"><span data-stu-id="81cf0-112">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="81cf0-113">HKEY_LOCAL_MACHINE\Security</span><span class="sxs-lookup"><span data-stu-id="81cf0-113">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="81cf0-114">HKEY_LOCAL_MACHINE\Software</span><span class="sxs-lookup"><span data-stu-id="81cf0-114">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="81cf0-115">HKEY_LOCAL_MACHINE\System</span><span class="sxs-lookup"><span data-stu-id="81cf0-115">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="81cf0-116">HKEY_USERS\\.Default.</span><span class="sxs-lookup"><span data-stu-id="81cf0-116">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="81cf0-117">可能な値は、`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSamSoftware`、`localMachineSystem`、`usersDefault` です。</span><span class="sxs-lookup"><span data-stu-id="81cf0-117">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="81cf0-118">Key</span><span class="sxs-lookup"><span data-stu-id="81cf0-118">key</span></span>|<span data-ttu-id="81cf0-119">文字列</span><span class="sxs-lookup"><span data-stu-id="81cf0-119">String</span></span>|<span data-ttu-id="81cf0-120">現在の (つまり変更された) 登録キー (独占HIVE)。</span><span class="sxs-lookup"><span data-stu-id="81cf0-120">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="81cf0-121">oldKey</span><span class="sxs-lookup"><span data-stu-id="81cf0-121">oldKey</span></span>|<span data-ttu-id="81cf0-122">文字列</span><span class="sxs-lookup"><span data-stu-id="81cf0-122">String</span></span>|<span data-ttu-id="81cf0-123">手前の (つまり変更される前)登録キー (独占HIVE)。</span><span class="sxs-lookup"><span data-stu-id="81cf0-123">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="81cf0-124">oldValueData</span><span class="sxs-lookup"><span data-stu-id="81cf0-124">oldValueData</span></span>|<span data-ttu-id="81cf0-125">文字列</span><span class="sxs-lookup"><span data-stu-id="81cf0-125">String</span></span>|<span data-ttu-id="81cf0-126">手前の (つまり変更される前)登録キーの値のデータ (内容).</span><span class="sxs-lookup"><span data-stu-id="81cf0-126">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="81cf0-127">oldValueName</span><span class="sxs-lookup"><span data-stu-id="81cf0-127">oldValueName</span></span>|<span data-ttu-id="81cf0-128">文字列</span><span class="sxs-lookup"><span data-stu-id="81cf0-128">String</span></span>|<span data-ttu-id="81cf0-129">手前の (つまり変更される前)登録キーの値の名前。</span><span class="sxs-lookup"><span data-stu-id="81cf0-129">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="81cf0-130">操作</span><span class="sxs-lookup"><span data-stu-id="81cf0-130">operation</span></span>|<span data-ttu-id="81cf0-131">registryOperation</span><span class="sxs-lookup"><span data-stu-id="81cf0-131">registryOperation</span></span>|<span data-ttu-id="81cf0-132">登録キーの名前および/または値を変更した操作。</span><span class="sxs-lookup"><span data-stu-id="81cf0-132">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="81cf0-133">可能な値は、`unknown`、`create`、`modify`、`delete` です。</span><span class="sxs-lookup"><span data-stu-id="81cf0-133">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="81cf0-134">processId</span><span class="sxs-lookup"><span data-stu-id="81cf0-134">processId</span></span>|<span data-ttu-id="81cf0-135">Int32</span><span class="sxs-lookup"><span data-stu-id="81cf0-135">Int32</span></span>|<span data-ttu-id="81cf0-136">登録キーを調整したプロセスのプロセスID (PID)(プロセスの詳細は警告「プロセス」コレクションに表示されます).</span><span class="sxs-lookup"><span data-stu-id="81cf0-136">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="81cf0-137">valueData</span><span class="sxs-lookup"><span data-stu-id="81cf0-137">valueData</span></span>|<span data-ttu-id="81cf0-138">文字列</span><span class="sxs-lookup"><span data-stu-id="81cf0-138">String</span></span>|<span data-ttu-id="81cf0-139">現在の (つまり変更された)登録キーの値のデータ(内容).</span><span class="sxs-lookup"><span data-stu-id="81cf0-139">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="81cf0-140">valueName</span><span class="sxs-lookup"><span data-stu-id="81cf0-140">valueName</span></span>|<span data-ttu-id="81cf0-141">文字列</span><span class="sxs-lookup"><span data-stu-id="81cf0-141">String</span></span>|<span data-ttu-id="81cf0-142">現在の (つまり変更された)登録キーの値の名前</span><span class="sxs-lookup"><span data-stu-id="81cf0-142">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="81cf0-143">valueType</span><span class="sxs-lookup"><span data-stu-id="81cf0-143">valueType</span></span>|<span data-ttu-id="81cf0-144">registryValueType</span><span class="sxs-lookup"><span data-stu-id="81cf0-144">registryValueType</span></span>|[<span data-ttu-id="81cf0-145">登録キーの値の種類</span><span class="sxs-lookup"><span data-stu-id="81cf0-145">Registry key value type</span></span>](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="81cf0-146">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="81cf0-146">REG_BINARY</span></span></li> <li><span data-ttu-id="81cf0-147">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="81cf0-147">REG_DWORD</span></span></li> <li><span data-ttu-id="81cf0-148">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="81cf0-148">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="81cf0-149">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="81cf0-149">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="81cf0-150">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="81cf0-150">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="81cf0-151">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="81cf0-151">REG_LINK</span></span></li> <li><span data-ttu-id="81cf0-152">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="81cf0-152">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="81cf0-153">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="81cf0-153">REG_NONE</span></span></li> <li><span data-ttu-id="81cf0-154">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="81cf0-154">REG_QWORD</span></span></li> <li><span data-ttu-id="81cf0-155">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="81cf0-155">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="81cf0-156">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="81cf0-156">REG_SZ</span></span></li></ul> <span data-ttu-id="81cf0-157">可能な値は、`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz` です。</span><span class="sxs-lookup"><span data-stu-id="81cf0-157">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81cf0-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="81cf0-158">JSON representation</span></span>

<span data-ttu-id="81cf0-159">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="81cf0-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->