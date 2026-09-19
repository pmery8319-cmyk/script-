local L=game:GetService("Lighting")
L.GlobalShadows=false
L.FogEnd=100000
for _,v in ipairs(L:GetChildren()) do
 if v:IsA("PostEffect") then v.Enabled=false end
end
for _,v in ipairs(workspace:GetDescendants()) do
 if v:IsA("ParticleEmitter") or v:IsA("Trail") then v.Enabled=false end
end
